# Getting and Cleaning Data Assigment 4
Repo created for Coursera Getting and Cleaning Data Assignment 4
****************************************************************
This repo contains data, CodeBook and R script used to download and clean the 'Human Activity Recognition Using Smartphones Dataset Version 1.0'. The raw data represent measurements collected from accelerometers from the Samsung Galaxy S smartphone. The cleaned data file represents a tidy dataset containing mean values grouped by subject and activity. A full description is available at the UCI machine learning repository where the data was obtained:

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

The source data can be found at this link

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

Reference for this study:
Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. Human Activity Recognition on Smartphones using a Multiclass Hardware-Friendly Support Vector Machine. International Workshop of Ambient Assisted Living (IWAAL 2012). Vitoria-Gasteiz, Spain. Dec 2012
*****************************************************

## Repo Contents
- R script to clean the data: run_analysis.R
- Tidy dataset containing mean values grouped by subject and activity: Means by Subject and Activity.csv
- code book explaining the variables from the tidy dataset :CodeBook.md
- this file: README.md

## R Analysis steps
run_analysis.R performs the following steps, resulting in an output subfolder called "data" that contains the source data, and a new tidy dataset called Means by Subject and Activity.csv. 

1. Downloads the data zip file from the UCI site 
2. Unzips the source file
3. Reads the source data files into R for both training and test datasets.
4. Combines columns and rows for the above datasets into a single data frame.
5. Adds column names using labels from the source file called features.txt
6. Extracts only the variables for the mean() or std()
7. Merges activity names from the file called activity_label.txt
8. Cleans up variable names by conversion to lower case, removal of extra characters, and expansion of abbreviations to be more understandable. These variable names are described in features_info.txt
9. Creates a new tidy dataset with the average of each variable for each activity and subject group.
10. Exports the dataset to 'Means by Subject and Activity.csv'. See CodeBook.md for explanation of the new variables.
