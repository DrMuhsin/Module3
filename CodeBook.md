

<p>CODE BOOK</p>

<h1></h1>

<p>UNITS OF MEASUREMENT OF VARIABLES </p>

<p>A full description on the methodology of collecting and computing the raw data is available at the site where the data was obtained: </p>

<p><a href="http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones#">http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones#</a></p>

<p>Features in the raw data are normalized and bounded within [-1,1].</p>

<h1></h1>

<p>TRANSFORMATION PERFORMED TO CLEAN UP THE RAW DATA</p>

<ul>
<li>Raw data files ("X_train.txt", "X_test.txt", "y_train.txt", "y_test.txt", "subject_train.txt", "subject_test.txt") were merged to create a single data frame.</li>
<li>The merged dataset was subset for 68 columns:

<ul>
<li>column containing activity code</li>
<li>column containing subject IDs</li>
<li>66 columns containing mean and standard deviation features</li>
</ul></li>
<li>Data set has been labelled with descriptive variable names (descriptive feature labels were sourced from 'features.txt' raw data file</li>
<li>An additional column was added to contain activity labels</li>
<li>By melting and casting the data set, an independent tidy data set has been created with the average of each 66 variables for each activity and each subject</li>
</ul>

<h1></h1>

<p>VARIABLE DICTIONARY</p>

<p>VARIABLE NAME           VARIABLE DESCRIPTION</p>

<p>Activity            The activity performed by the volunteers while wearing a smartphone (Samsung Galaxy S II) on the waist during the experiment (the 6 activities performed are: WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING).</p>

<p>SubjectID           The unique identifier of the subject (there were 30 volunteers participating in the experiment) who performed the activity for each window sample.</p>

<p>tBodyAcc-mean()-X       The average of the mean values of the body acceleration time domain signals from the smartphone accelerometer X axis for a given activity and a given subject.  </p>

<p>tBodyAcc-mean()-Y       The average of the mean values of the body acceleration time domain signals from the smartphone accelerometer Y axis for a given activity and a given subject.  </p>

<p>tBodyAcc-mean()-Z       The average of the mean values of the body acceleration time domain signals from the smartphone accelerometer Z axis for a given activity and a given subject.  </p>

<p>tGravityAcc-mean()-X        The average of the mean values of the gravity acceleration time domain signals from the smartphone accelerometer X axis for a given activity and a given subject.   </p>

<p>tGravityAcc-mean()-Y        The average of the mean values of the gravity acceleration time domain signals from the smartphone accelerometer Y axis for a given activity and a given subject.</p>

<p>tGravityAcc-mean()-Z        The average of the mean values of the gravity acceleration time domain signals from the smartphone accelerometer Z axis for a given activity and a given subject.</p>

<p>tBodyAccJerk-mean()-X       The average of the mean values of the body acceleration time domain jerk signals from the smartphone accelerometer X axis for a given activity and a given subject.</p>

<p>tBodyAccJerk-mean()-Y       The average of the mean values of the body acceleration time domain jerk signals from the smartphone accelerometer Y axis for a given activity and a given subject.</p>

<p>tBodyAccJerk-mean()-Z       The average of the mean values of the body acceleration time domain jerk signals from the smartphone accelerometer Z axis for a given activity and a given subject.</p>

<p>tBodyGyro-mean()-X      The average of the mean values of the body acceleration time domain signals from the smartphone gyroscope X axis for a given activity and a given subject.</p>

<p>tBodyGyro-mean()-Y      The average of the mean values of the body acceleration time domain signals from the smartphone gyroscope Y axis for a given activity and a given subject.</p>

<p>tBodyGyro-mean()-Z      The average of the mean values of the body acceleration time domain signals from the smartphone gyroscope Z axis for a given activity and a given subject.</p>

<p>tBodyGyroJerk-mean()-X      The average of the mean values of the body acceleration time domain jerk signals from the smartphone gyroscope X axis for a given activity and a given subject.</p>

<p>tBodyGyroJerk-mean()-Y      The average of the mean values of the body acceleration time domain jerk signals from the smartphone gyroscope Y axis for a given activity and a given subject.</p>

<p>tBodyGyroJerk-mean()-Z      The average of the mean values of the body acceleration time domain jerk signals from the smartphone gyroscope Z axis for a given activity and a given subject.</p>

<p>tBodyAccMag-mean()      The average of the mean values of the magnitude of three-dimensional body acceleration time domain signals from the smartphone accelerometer for a given activity and a given subject.</p>

<p>tGravityAccMag-mean()       The average of the mean values of the magnitude of three-dimensional gravity acceleration time domain signals from the smartphone accelerometer for a given activity and a given subject.</p>

<p>tBodyAccJerkMag-mean()      The average of the mean values of the magnitude of three-dimensional body acceleration time domain jerk signals from the smartphone accelerometer for a given activity and a given subject.</p>

<p>tBodyGyroMag-mean()     The average of the mean values of the magnitude of three-dimensional body acceleration time domain signals from the smartphone gyroscope for a given activity and a given subject.</p>

<p>tBodyGyroJerkMag-mean()     The average of the mean values of the magnitude of three-dimensional body acceleration time domain jerk signals from the smartphone gyroscope for a given activity and a given subject.</p>

<p>fBodyAcc-mean()-X       The average of the mean values of the body acceleration frequency domain signals from the smartphone accelerometer X axis for a given activity and a given subject.     </p>

<p>fBodyAcc-mean()-Y       The average of the mean values of the body acceleration frequency domain signals from the smartphone accelerometer Y axis for a given activity and a given subject.</p>

<p>fBodyAcc-mean()-Z       The average of the mean values of the body acceleration frequency domain signals from the smartphone accelerometer Z axis for a given activity and a given subject.</p>

<p>fBodyAccJerk-mean()-X       The average of the mean values of the body acceleration frequency domain jerk signals from the smartphone accelerometer X axis for a given activity and a given subject.</p>

<p>fBodyAccJerk-mean()-Y       The average of the mean values of the body acceleration frequency domain jerk signals from the smartphone accelerometer Y axis for a given activity and a given subject.</p>

<p>fBodyAccJerk-mean()-Z       The average of the mean values of the body acceleration frequency domain jerk signals from the smartphone accelerometer Z axis for a given activity and a given subject.</p>

<p>fBodyGyro-mean()-X      The average of the mean values of the body acceleration frequency domain signals from the smartphone gyroscope X axis for a given activity and a given subject.</p>

<p>fBodyGyro-mean()-Y      The average of the mean values of the body acceleration frequency domain signals from the smartphone gyroscope Y axis for a given activity and a given subject.</p>

<p>fBodyGyro-mean()-Z      The average of the mean values of the body acceleration frequency domain signals from the smartphone gyroscope Z axis for a given activity and a given subject.</p>

<p>fBodyAccMag-mean()      The average of the mean values of the magnitude of three-dimensional body acceleration frequency domain signals from the smartphone accelerometer for a given activity and a given subject. </p>

<p>fBodyBodyAccJerkMag-mean()  The average of the mean values of the magnitude of three-dimensional body acceleration frequency domain jerk signals from the smartphone accelerometer for a given activity and a given subject.</p>

<p>fBodyBodyGyroMag-mean()     The average of the mean values of the magnitude of three-dimensional body acceleration frequency domain signals from the smartphone gyroscope for a given activity and a given subject.</p>

<p>fBodyBodyGyroJerkMag-mean() The average of the mean values of the magnitude of three-dimensional body acceleration frequency domain jerk signals from the smartphone gyroscope for a given activity and a given subject.</p>

<p>tBodyAcc-std()-X        The average of the standard deviation values of the body acceleration time domain signals from the smartphone accelerometer X axis for a given activity and a given subject.</p>

<p>tBodyAcc-std()-Y        The average of the standard deviation values of the body acceleration time domain signals from the smartphone accelerometer Y axis for a given activity and a given subject.</p>

<p>tBodyAcc-std()-Z        The average of the standard deviation values of the body acceleration time domain signals from the smartphone accelerometer Z axis for a given activity and a given subject.</p>

<p>tGravityAcc-std()-X     The average of the standard deviation values of the gravity acceleration time domain signals from the smartphone accelerometer X axis for a given activity and a given subject.</p>

<p>tGravityAcc-std()-Y     The average of the standard deviation values of the gravity acceleration time domain signals from the smartphone accelerometer Y axis for a given activity and a given subject.</p>

<p>tGravityAcc-std()-Z     The average of the standard deviation values of the gravity acceleration time domain signals from the smartphone accelerometer Z axis for a given activity and a given subject.</p>

<p>tBodyAccJerk-std()-X        The average of the standard deviation values of the body acceleration time domain jerk signals from the smartphone accelerometer X axis for a given activity and a given subject.</p>

<p>tBodyAccJerk-std()-Y        The average of the standard deviation values of the body acceleration time domain jerk signals from the smartphone accelerometer Y axis for a given activity and a given subject.</p>

<p>tBodyAccJerk-std()-Z        The average of the standard deviation values of the body acceleration time domain jerk signals from the smartphone accelerometer Z axis for a given activity and a given subject.</p>

<p>tBodyGyro-std()-X       The average of the standard deviation values of the body acceleration time domain signals from the smartphone gyroscope X axis for a given activity and a given subject.</p>

<p>tBodyGyro-std()-Y       The average of the standard deviation values of the body acceleration time domain signals from the smartphone gyroscope Y axis for a given activity and a given subject.</p>

<p>tBodyGyro-std()-Z       The average of the standard deviation values of the body acceleration time domain signals from the smartphone gyroscope Z axis for a given activity and a given subject.</p>

<p>tBodyGyroJerk-std()-X       The average of the standard deviation values of the body acceleration time domain jerk signals from the smartphone gyroscope X axis for a given activity and a given subject.</p>

<p>tBodyGyroJerk-std()-Y       The average of the standard deviation values of the body acceleration time domain jerk signals from the smartphone gyroscope Y axis for a given activity and a given subject.</p>

<p>tBodyGyroJerk-std()-Z       The average of the standard deviation values of the body acceleration time domain jerk signals from the smartphone gyroscope Z axis for a given activity and a given subject.</p>

<p>tBodyAccMag-std()       The average of the standard deviation values of the magnitude of three-dimensional body acceleration time domain signals from the smartphone accelerometer for a given activity and a given subject.</p>

<p>tGravityAccMag-std()        The average of the standard deviation values of the magnitude of three-dimensional gravity acceleration time domain signals from the smartphone accelerometer for a given activity and a given subject.</p>

<p>tBodyAccJerkMag-std()       The average of the standard deviation values of the magnitude of three-dimensional body acceleration time domain jerk signals from the smartphone accelerometer for a given activity and a given subject.</p>

<p>tBodyGyroMag-std()      The average of the standard deviation values of the magnitude of three-dimensional body acceleration time domain signals from the smartphone gyroscope for a given activity and a given subject.</p>

<p>tBodyGyroJerkMag-std()      The average of the standard deviation values of the magnitude of three-dimensional body acceleration time domain jerk signals from the smartphone gyroscope for a given activity and a given subject.</p>

<p>fBodyAcc-std()-X        The average of the standard deviation values of the body acceleration frequency domain signals from the smartphone accelerometer X axis for a given activity and a given subject.</p>

<p>fBodyAcc-std()-Y        The average of the standard deviation values of the body acceleration frequency domain signals from the smartphone accelerometer Y axis for a given activity and a given subject.</p>

<p>fBodyAcc-std()-Z        The average of the standard deviation values of the body acceleration frequency domain signals from the smartphone accelerometer Z axis for a given activity and a given subject.</p>

<p>fBodyAccJerk-std()-X        The average of the standard deviation values of the body acceleration frequency domain jerk signals from the smartphone accelerometer X axis for a given activity and a given subject.</p>

<p>fBodyAccJerk-std()-Y        The average of the standard deviation values of the body acceleration frequency domain jerk signals from the smartphone accelerometer Y axis for a given activity and a given subject.</p>

<p>fBodyAccJerk-std()-Z        The average of the standard deviation values of the body acceleration frequency domain jerk signals from the smartphone accelerometer Z axis for a given activity and a given subject.</p>

<p>fBodyGyro-std()-X       The average of the standard deviation values of the body acceleration frequency domain signals from the smartphone gyroscope X axis for a given activity and a given subject.</p>

<p>fBodyGyro-std()-Y       The average of the standard deviation values of the body acceleration frequency domain signals from the smartphone gyroscope Y axis for a given activity and a given subject.</p>

<p>fBodyGyro-std()-Z       The average of the standard deviation values of the body acceleration frequency domain signals from the smartphone gyroscope Z axis for a given activity and a given subject.</p>

<p>fBodyAccMag-std()       The average of the standard deviation values of the magnitude of three-dimensional body acceleration frequency domain signals from the smartphone accelerometer for a given activity and a given subject.</p>

<p>fBodyBodyAccJerkMag-std()   The average of the standard deviation values of the magnitude of three-dimensional body acceleration frequency domain jerk signals from the smartphone accelerometer for a given activity and a given subject.</p>

<p>fBodyBodyGyroMag-std()      The average of the standard deviation values of the magnitude of three-dimensional body acceleration frequency domain signals from the smartphone gyroscope for a given activity and a given subject.</p>

<p>fBodyBodyGyroJerkMag-std()  The average of the standard deviation values of the magnitude of three-dimensional body acceleration frequency domain jerk signals from the smartphone gyroscope for a given activity and a given subject.</p>

<p>NOTE: for additional information on the experiment and the calculation of the above variables please visit the following website: 
<a href="http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones">http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones</a></p>
</article>
  </div>

