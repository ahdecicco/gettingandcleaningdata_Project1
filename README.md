gettingandcleaningdata_Project1
===============================

Repo_DataSci_3_Proj_1
=====================

Getting and Cleaning Data Course; repo for project 1.

<h3>PROJECT DESCRIPTION

This repository contains data, instructions, a runnable R script, and a codebook to use with Project 1 of the Getting and Cleaning Data Course through Coursera. 

The data used for this project, and used by the script, can be found as a zip file at the following url:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

A description of the data is contained in the 'codebook' file in this repository, and a more detailed description of the data can be found at this url:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 


<h3>THE SCRIPT

The run_analysis.R script first loads the data from the UCI HAR Dataset, and assumes the file structure is unchanged after unzipping the dataset into the working directory.

The script loads all data files from the "Test" subdirectory first; x_test.txt, y_test.txt, and subject_test.txt. It then repeats this for the "Train" subdirectory. Finally, the activity_labels.txt and features.txt files are loaded.

the script assigns names to all the data columns of the index files (y_ and subject_ and activity_labels files), and assigns column names to the data itself using the features.txt file.

The data sets is first merged into two dataframes; one for the test data and one for the training data, using cbind(). Next the raining and test data frames are merged using rbind(). At this point, all raw data has been merged into a single dataframe.

Following tidy data principles, we use descriptive activity labels instead of a non-descript activity index number. To create descriptive activity names we (1) merge the now complete dataframe with the activity_labels data , merging by the activity index, and we (2) delete the column for activity number index since we don't need this.

For this project, we only need features that are mean and std dev variables, so we just extract those columns from the aggregate dataframe using the grep1() function, and use the result to subset the data as a filtered dataframe. We then output this filtered data using write.table().

Lastly, to complete the project, we create a single, independent, tidy data set that is a summary of the data frame of the mean and std dev variables, summarized using the average of each variable for each activity and each subject. We use the aggregate() function to create this second, smaller, tidy data set. The output is writted to a *.txt file that has comma separated values (csv).
