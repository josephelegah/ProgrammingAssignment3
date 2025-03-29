# ProgrammingAssignment3
R tidy data
# ProgrammingAssignment3
R tidy data
# Getting and Cleaning Data Course Project

This repository contains the R script `run_analysis.R` and the resulting tidy data set `tidydata.txt` for the "Getting and Cleaning Data" course project.

## Project Description

The goal of this project was to collect, work with, and clean a data set from the UCI Machine Learning Repository. The data set used was the "Human Activity Recognition Using Smartphones" data set, which contains data collected from accelerometers and gyroscopes of Samsung Galaxy S II smartphones.

The `run_analysis.R` script performs the following tasks:

1.  **Downloads and unzips the data set:** If the data set is not already present, it is downloaded from the provided URL and unzipped.
2.  **Reads the data:** The training and test data sets, along with the activity labels and feature names, are read into R.
3.  **Merges the training and test sets:** The training and test data sets are merged into a single data set.
4.  **Extracts mean and standard deviation measurements:** Only the measurements on the mean and standard deviation for each measurement are extracted.
5.  **Uses descriptive activity names:** The activity labels are used to name the activities in the data set.
6.  **Labels the data set with descriptive variable names:** The variable names are made more descriptive and readable.
7.  **Creates a tidy data set:** A second, independent tidy data set is created with the average of each variable for each activity and each subject.
8.  **Writes the tidy data set to a file:** The tidy data set is written to a text file named `tidydata.txt`.

## Files

* `run_analysis.R`: The R script that performs the data cleaning and analysis.
* `tidydata.txt`: The resulting tidy data set.
* `CodeBook.md`: Contains the variable names, data types, and descriptions of the data found in tidydata.txt

## Running the Script

1.  Ensure you have R and RStudio installed.
2.  Download or clone this repository.
3.  Place `run_analysis.R` in your desired working directory.
4.  Open RStudio and set the working directory to the location of `run_analysis.R`.
5.  Run the script using `source("run_analysis.R")`.
6.  The `tidydata.txt` file will be created in the same directory.

## Code Book (`CodeBook.md`)

The `CodeBook.md` file provides detailed information about the variables in the `tidydata.txt` file, including:

* Variable names and descriptions
* Units of measurement (where applicable)
* Data types
* The calculations that were performed to derive the tidy data.

It is crucial to consult the code book to properly interpret the data in `tidydata.txt`.

## Notes

* The `dplyr` package is required to run the script. Install it using `install.packages("dplyr")` if it is not already installed.
* The data set is downloaded from the following URL: `https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip`

This README provides a clear and concise overview of the project and its files. It should allow anyone to easily understand and reproduce the analysis.
