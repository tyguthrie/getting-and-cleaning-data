# Codebook for 'Means by Subject and Activity.csv'

## Source Variable Description
The orginal variables are from the 'Human Activity Recognition Using Smartphones Dataset Version 1.0'. The feature_info.txt file from that dataset provides the following description of the source variables.
**********************************
>The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 
>
>Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 
>
>Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 
>
>These signals were used to estimate variables of the feature vector for each pattern: '-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

## Variables
The following table describes the new tidy variable, the original source variable and the transformation. Only the variables used in the final output are listed here. See the  'features.txt' file for list of all source variables included in the original dataset. The original test and training datasets were combined. All new variables represent mean values grouped by subject and activity.
********************************
New Variable | Original Variable | Transformation
--- | --- | ---
subject | subjects_test/train.txt | combined train and test datasets
activity | activities from activities.txt | joined to activity codes
time domain body accelerometer mean x axis | tBodyAcc-mean()-X | mean by subject/activity
time domain body accelerometer mean y axis | tBodyAcc-mean()-Y | mean by subject/activity
time domain body accelerometer mean z axis | tBodyAcc-mean()-Z | mean by subject/activity
time domain body accelerometer standard deviation x axis | tBodyAcc-std()-X | mean by subject/activity
time domain body accelerometer standard deviation y axis | tBodyAcc-std()-Y | mean by subject/activity
time domain body accelerometer standard deviation z axis | tBodyAcc-std()-Z | mean by subject/activity
time domain gravity accelerometer mean x axis | tGravityAcc-mean()-X | mean by subject/activity
time domain gravity accelerometer mean y axis | tGravityAcc-mean()-Y | mean by subject/activity
time domain gravity accelerometer mean z axis | tGravityAcc-mean()-Z | mean by subject/activity
time domain gravity accelerometer standard deviation x axis | tGravityAcc-std()-X | mean by subject/activity
time domain gravity accelerometer standard deviation y axis | tGravityAcc-std()-Y | mean by subject/activity
time domain gravity accelerometer standard deviation z axis | tGravityAcc-std()-Z | mean by subject/activity
time domain body accelerometer jerk mean x axis | tBodyAccJerk-mean()-X | mean by subject/activity
time domain body accelerometer jerk mean y axis | tBodyAccJerk-mean()-Y | mean by subject/activity
time domain body accelerometer jerk mean z axis | tBodyAccJerk-mean()-Z | mean by subject/activity
time domain body accelerometer jerk standard deviation x axis | tBodyAccJerk-std()-X | mean by subject/activity
time domain body accelerometer jerk standard deviation y axis | tBodyAccJerk-std()-Y | mean by subject/activity
time domain body accelerometer jerk standard deviation z axis | tBodyAccJerk-std()-Z | mean by subject/activity
time domain body gyroscope mean x axis | tBodyGyro-mean()-X | mean by subject/activity
time domain body gyroscope mean y axis | tBodyGyro-mean()-Y | mean by subject/activity
time domain body gyroscope mean z axis | tBodyGyro-mean()-Z | mean by subject/activity
time domain body gyroscope standard deviation x axis | tBodyGyro-std()-X | mean by subject/activity
time domain body gyroscope standard deviation y axis | tBodyGyro-std()-Y | mean by subject/activity
time domain body gyroscope standard deviation z axis | tBodyGyro-std()-Z | mean by subject/activity
time domain body gyroscope jerk mean x axis | tBodyGyroJerk-mean()-X | mean by subject/activity
time domain body gyroscope jerk mean y axis | tBodyGyroJerk-mean()-Y | mean by subject/activity
time domain body gyroscope jerk mean z axis | tBodyGyroJerk-mean()-Z | mean by subject/activity
time domain body gyroscope jerk standard deviation x axis | tBodyGyroJerk-std()-X | mean by subject/activity
time domain body gyroscope jerk standard deviation y axis | tBodyGyroJerk-std()-Y | mean by subject/activity
time domain body gyroscope jerk standard deviation z axis | tBodyGyroJerk-std()-Z | mean by subject/activity
time domain body accelerometer magnitude mean | tBodyAccMag-mean() | mean by subject/activity
time domain body accelerometer magnitude standard deviation | tBodyAccMag-std() | mean by subject/activity
time domain gravity accelerometer magnitude mean | tGravityAccMag-mean() | mean by subject/activity
time domain gravity accelerometer magnitude standard deviation | tGravityAccMag-std() | mean by subject/activity
time domain body accelerometer jerk magnitude mean | tBodyAccJerkMag-mean() | mean by subject/activity
time domain body accelerometer jerk magnitude standard deviation | tBodyAccJerkMag-std() | mean by subject/activity
time domain body gyroscope magnitude mean | tBodyGyroMag-mean() | mean by subject/activity
time domain body gyroscope magnitude standard deviation | tBodyGyroMag-std() | mean by subject/activity
time domain body gyroscope jerk magnitude mean | tBodyGyroJerkMag-mean() | mean by subject/activity
time domain body gyroscope jerk magnitude standard deviation | tBodyGyroJerkMag-std() | mean by subject/activity
frequency domain body accelerometer mean x axis | fBodyAcc-mean()-X | mean by subject/activity
frequency domain body accelerometer mean y axis | fBodyAcc-mean()-Y | mean by subject/activity
frequency domain body accelerometer mean z axis | fBodyAc-mean()c-Z | mean by subject/activity
frequency domain body accelerometer standard deviation x axis | fBodyAcc-std()-X | mean by subject/activity
frequency domain body accelerometer standard deviation y axis | fBodyAcc-std()-Y | mean by subject/activity
frequency domain body accelerometer standard deviation z axis | fBodyAcc-std()-Z | mean by subject/activity
frequency domain body accelerometer mean frequency x axis | fBodyAcc-meanFreq()-X | mean by subject/activity
frequency domain body accelerometer mean frequency y axis | fBodyAcc-meanFreq()-Y | mean by subject/activity
frequency domain body accelerometer mean frequency z axis | fBodyAcc-meanFreq()-Z | mean by subject/activity
frequency domain body accelerometer jerk mean x axis | fBodyAccJerk-mean()-X | mean by subject/activity
frequency domain body accelerometer jerk mean y axis | fBodyAccJerk-mean()-Y | mean by subject/activity
frequency domain body accelerometer jerk mean z axis | fBodyAccJerk-mean()-Z | mean by subject/activity
frequency domain body accelerometer jerk standard deviation x axis | fBodyAccJerk-std()-X | mean by subject/activity
frequency domain body accelerometer jerk standard deviation y axis | fBodyAccJerk-std()-Y | mean by subject/activity
frequency domain body accelerometer jerk standard deviation z axis | fBodyAccJerk-std()-Z | mean by subject/activity
frequency domain body accelerometer jerk mean frequency x axis | fBodyAccJerk-mean()-X | mean by subject/activity
frequency domain body accelerometer jerk mean frequency y axis | fBodyAccJerk-mean()-Y | mean by subject/activity
frequency domain body accelerometer jerk mean frequency z axis | fBodyAccJerk-mean()-Z | mean by subject/activity
frequency domain body gyroscope mean x axis | fBodyGyro-mean()-X | mean by subject/activity
frequency domain body gyroscope mean y axis | fBodyGyro-mean()-Y | mean by subject/activity
frequency domain body gyroscope mean z axis | fBodyGyro-mean()-Z | mean by subject/activity
frequency domain body gyroscope standard deviation x axis | fBodyGyro-std()-X | mean by subject/activity
frequency domain body gyroscope standard deviation y axis | fBodyGyro-std()-Y | mean by subject/activity
frequency domain body gyroscope standard deviation z axis | fBodyGyro-std()-Z | mean by subject/activity
frequency domain body gyroscope mean frequency x axis | fBodyGyro-meanFreq()-X | mean by subject/activity
frequency domain body gyroscope mean frequency y axis | fBodyGyro-meanFreq()-Y | mean by subject/activity
frequency domain body gyroscope mean frequency z axis | fBodyGyro-meanFreq()-Z | mean by subject/activity
frequency domain body accelerometer magnitude mean | fBodyAccMag-mean() | mean by subject/activity
frequency domain body accelerometer magnitude standard deviation | fBodyAccMag-std() | mean by subject/activity
frequency domain body accelerometer magnitude mean frequency | fBodyBodyAccJerkMag-meanFreq() | mean by subject/activity
frequency domain body accelerometer jerk magnitude mean | fBodyAccJerkMag-mean() | mean by subject/activity
frequency domain body accelerometer jerk magnitude standard deviation | fBodyAccJerkMag-std() | mean by subject/activity
frequency domain body accelerometer jerk magnitude mean frequency | fBodyBodyAccJerkMag-meanFreq() | mean by subject/activity
frequency domain body gyroscope magnitude mean | fBodyGyroMag-mean() | mean by subject/activity
frequency domain body gyroscope magnitude standard deviation | fBodyGyroMag-std() | mean by subject/activity
frequency domain body gyroscope magnitude mean frequency | fBodyBodyGyroMag-meanFreq() | mean by subject/activity
frequency domain body gyroscope jerk magnitude mean | fBodyGyroJerkMag-mean() | mean by subject/activity
frequency domain body gyroscope jerk magnitude standard deviation | fBodyGyroJerkMag-std() | mean by subject/activity
frequency domain body gyroscope jerk magnitude mean frequency | fBodyBodyGyroJerkMag-meanFreq() | mean by subject/activity











