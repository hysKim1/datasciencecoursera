# Getting and Cleaning Data Project(Coursera)

## Code is written in R in file. Source file is `run_analysis.R `which consists of the following 5 steps:
### Download the dataset if it does not already exist in the working directory and unzip. 
### List all the files of `UCI HAR Dataset` folder and load data are listed
	`test/subject_test.txt`	
	`test/X_test.txt`
	`test/y_test.txt`
	`train/subject_train.txt`
	`train/X_train.txt`
	`train/y_train.txt`
	
### Load activity, subject and feature info and read data from the files into the variables: 
		
1. Merges the training and the test sets to create one data set.
	* Concatenate the data tables by rows.
	* set names to variables.
	* Merge columns to get the data frame Data for all data.
	
2. Extracts only the measurements on the mean and standard deviation for each measurement.
	* Subset Name of Features by measurements on the mean and standard deviation.
	* Subset the data frame Data by selected names of Features.
	
3. Uses descriptive activity names to name the activities in the data set.
	* Read descriptive activity names from `activity_labels.txt`
	* Factorize variable activity in the data frame Data using descriptive activity names.
	
4. Appropriately labels the data set with descriptive variable names.

5. Creates a second, independent tidy dataset with the average of each variable for each activity and each subject.
*Final output file is `tidydata.txt`
