# Coursera_Module3_Assignment
Data Science Coursera Module 3 Getting and Cleaning Data 

# Introduction
This is the assignment from the Module 3, Getting and Cleaning Data of the Data Science Specialization
Data was obtained from [here](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip).
It was manually downloaded and unzipped. ReadMe file from the dataset describes the data and variables.

In this assignment, 3 files were submitted for peer grading:

- [README.md](https://github.com/xingruoyu/Coursera_Module3_Assignment/blob/master/README.md)
- [run_analysis.R](https://github.com/xingruoyu/Coursera_Module3_Assignment/blob/master/run_analysis.R)
- [CodeBook.md](https://github.com/xingruoyu/Coursera_Module3_Assignment/blob/master/CodeBook.md)

# How to check result "tidy.txt"
- Download the dataset, save and unzip under your direcoty
- Note: Do not change the name of the data folder, it should remain "UCI_HAR_Dataset"
- Open the script "run_analysis.R" in R studio and run
- Use command: read.table("tidy.txt", header = TRUE)

# Dependencies
- The R script assumes that the dplyr package was installed.

# Study design
- Import test data, subject id, feature(variable names) dataset into data frames
- Combine the above 3 dataset into one
- Perform same procedures to the train datasets
- Combine test and train dataset
- Extract dataset with variables with string "mean" and "std"
- Replaced activity IDs with the activity labels for readability
- Group the dataset based on subject IDs and activity
- Calculate mean for the new dataset, saving under "result"
- Write the "result" as "tidy.txt" as final output

# More information
You can find more info about this assignment from [here](https://www.coursera.org/learn/data-cleaning/peer/FIZtT/getting-and-cleaning-data-course-project).
