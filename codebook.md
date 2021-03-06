
Codebook
==================================================================

The data used in the script contained in this repository is described below. The text below is from a readme file created by the originators of the dataset, and is reproduced in its entirety below.The data itself can be found at the following location: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip.

<h4>Source</h4>
  * Jorge L. Reyes-Ortiz, Davide Anguita, Alessandro Ghio, Luca Oneto. 
  * Smartlab - Non Linear Complex Systems Laboratory 
  * DITEN - UniversitÃ  degli Studi di Genova, Genoa I-16145, Italy. 
  * activityrecognition '@' smartlab.ws 
  * www.smartlab.ws 
  
Original Data
-------------
The data contained here was originally generated by subjects using a wearable accelerometer and gyroscope. The process of generating the original data is described below, by the providers of the data at www.smartlab.ws. The full description can be found at: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones. 

"The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. See 'features_info.txt' for more details." 

That data can be found at https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip.

Processed Data
---------------
The data in this repository, generated by the script contained here, is a processed and filtered form of the original data. Only the variables containing mean or standard deviation measurements were retained from the original data. That data was aggregated into the dataset contained in this repository, by getting the mean of all the remaining data variables, for each subject and activity. There are 30 total subjects in the study, each performing six activities, so there are a total of 180 aggregate data values in the final data set.

Activities
---------------
The subjects in the study performed the following activities when the data was gathered:
<ul>
	<li>WALKING</li>
	<li>WALKING_UPSTAIRS</li>
	<li>WALKING_DOWNSTAIRS</li>
	<li>SITTING</li>
	<li>STANDING</li>
	<li>LAYING</li>
</ul>

Data Variables
--------------
The following data variables are contained in the processed data:
<ul>
<li>subject</li>
<li>activity</li>
<li>tBodyAcc_mean_X</li>
	<li>tBodyAcc_mean_Y</li>
        <li>tBodyAcc_mean_Z</li>
        <li>tBodyAcc_std_X</li>
        <li>tBodyAcc_std_Y</li>
	<li>tBodyAcc_std_Z</li>
	<li>tGravityAcc_mean_X</li>
        <li>tGravityAcc_mean_Y</li>
        <li>tGravityAcc_mean_Z</li>
        <li>tGravityAcc_std_X</li>
	<li>tGravityAcc_std_Y</li>
	<li>tGravityAcc_std_Z</li>
        <li>tBodyAccJerk_mean_X</li>
        <li>tBodyAccJerk_mean_Y</li>
        <li>tBodyAccJerk_mean_Z</li>
	<li>tBodyAccJerk_std_X</li>
	<li>tBodyAccJerk_std_Y</li>
        <li>tBodyAccJerk_std_Z</li>
        <li>tBodyGyro_mean_X</li>
        <li>tBodyGyro_mean_Y</li>
	<li>tBodyGyro_mean_Z</li>
	<li>tBodyGyro_std_X</li>
        <li>tBodyGyro_std_Y</li>
        <li>tBodyGyro_std_Z</li>
        <li>tBodyGyroJerk_mean_X</li>
	<li>tBodyGyroJerk_mean_Y</li>
	<li>tBodyGyroJerk_mean_Z</li>
        <li>tBodyGyroJerk_std_X</li>
        <li>tBodyGyroJerk_std_Y</li>
        <li>tBodyGyroJerk_std_Z</li>
	<li>tBodyAccMag_mean</li>
	<li>tBodyAccMag_std</li>
        <li>tGravityAccMag_mean</li>
        <li>tGravityAccMag_std</li>
        <li>tBodyAccJerkMag_mean</li>
	<li>tBodyAccJerkMag_std</li>
	<li>tBodyGyroMag_mean</li>
        <li>tBodyGyroMag_std</li>
        <li>tBodyGyroJerkMag_mean</li>
        <li>tBodyGyroJerkMag_std</li>
	<li>fBodyAcc_mean_X</li>
	<li>fBodyAcc_mean_Y</li>
        <li>fBodyAcc_mean_Z</li>
        <li>fBodyAcc_std_X</li>
        <li>fBodyAcc_std_Y</li>
	<li>fBodyAcc_std_Z</li>
	<li>fBodyAccJerk_mean_X</li>
        <li>fBodyAccJerk_mean_Y</li>
        <li>fBodyAccJerk_mean_Z</li>
        <li>fBodyAccJerk_std_X</li>
	<li>fBodyAccJerk_std_Y</li>
	<li>fBodyAccJerk_std_Z</li>
        <li>fBodyGyro_mean_X</li>
        <li>fBodyGyro_mean_Y</li>
        <li>fBodyGyro_mean_Z</li>
	<li>fBodyGyro_std_X</li>
	<li>fBodyGyro_std_Y</li>
        <li>fBodyGyro_std_Z</li>
        <li>fBodyAccMag_mean</li>
        <li>fBodyAccMag_std</li>
	<li>fBodyAccJerkMag_mean</li>
	<li>fBodyAccJerkMag_std</li>
        <li>fBodyGyroMag_mean</li>
        <li>fBodyGyroMag_std</li>
        <li>fBodyGyroJerkMag_mean</li>
	<li>fBodyGyroJerkMag_std</li>
	</ul>
