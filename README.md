---
title: "README.md"
author: "DrMuhsin"
date: "Sunday, August 23, 2015"
output: html_document
---

##First we Extract the dataset online
```{r}
onlineFile <- "https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip"
```

##download the file
```{r}
download.file(onlineFile, "./UCI-HAR-dataset.zip", method="auto")
```

##unzip the file
```{r}
unzip("./UCI-HAR-dataset.zip")
```



# Q1. Merges the training and the test sets to create one data set.
```{r}
##Read the features column
features <- read.table("./UCI HAR Dataset/features.txt")
##Read test.x data
test.x <- read.table("./UCI HAR Dataset/test/X_test.txt", col.names=features[,2])
##read train.x data
train.x <- read.table("./UCI HAR Dataset/train/X_train.txt", col.names=features[,2])
X <- rbind(test.x, train.x)
```



# Q2. Extracts only the measurements on the mean and standard deviation for each measurement. 
```{r}
##Filter features which has column mean and std since we only want the Mean and Standard Deviation
features <- features[grep("(mean|std)\\(", features[,2]),]
##add both to mean_and_std
mean_and_stdD <- X[,features[,1]]
```


# Q3. Uses descriptive activity names to name the activities in the data set
```{r}
##read test.y data
test.y <- read.table("./UCI HAR Dataset/test/y_test.txt", col.names = c('activity'))
##read train.y data
train.y <- read.table("./UCI HAR Dataset/train/y_train.txt", col.names = c('activity'))
##bind to y
y <- rbind(test.y, train.y)
```

##read labels provided
```{r}
labels <- read.table("./UCI HAR Dataset/activity_labels.txt")
```

##mapping codes
```{r}
for (i in 1:nrow(labels)) {
  code <- as.numeric(labels[i, 1])
  name <- as.character(labels[i, 2])
  y[y$activity == code, ] <- name
}
```



# Q4. Appropriately labels the data set with descriptive activity names. 
```{r}
##read labels.x
labels.x <- cbind(y, X)
##bind to labels.mean_and_std
labels.mean_and_std <- cbind(y, mean_and_stdD)
```


# Q5. Creates a second, independent tidy data set with the average of each variable for each activity and each subject. 
```{r}
##test.subject
test.subject <- read.table("./UCI HAR Dataset/test/subject_test.txt", col.names = c('subject'))
##train.subject
train.subject <- read.table("./UCI HAR Dataset/train/subject_train.txt", col.names = c('subject'))
## bind to subject
subject <- rbind(test.subject, train.subject)
## get average
averages <- aggregate(X, by = list(activity = y[,1], subject = subject[,1]), mean)
if (file.exists("./result.txt")){
  file.remove("./result.txt")
}
```



## write the results in text format. 
```{r}
write.csv(averages, file="./result.txt", row.names=FALSE)
```

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.
