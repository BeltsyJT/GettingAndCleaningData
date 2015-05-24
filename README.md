Requriements:

Create R script called run_analysis.R that does the following: 
- Merges the training and the test sets to create one data set.
- Extracts only the measurements on the mean and standard deviation for each measurement. 
- Uses descriptive activity names to name the activities in the data set
- Appropriately labels the data set with descriptive variable names. 
- From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

Dependencies:
run_analysis.R needs reshape2 and data.table packages to run correctly. Both packges are loaded automatically by the code.

Code Overview:

- Install neccesery packages
- Get activity labels file
- Get column names from features.txt
- Extract mean and standard deviation for each measurement.
- Get X_test, y_test, and subject_test files
- Extract mean and standard deviation for each measurement.
- Load activity labels
- Bind data
- Load and process X_train, y_train and subject_train files
- Extract only the measurements on the mean and standard deviation for each measurement.
- Load activity data
- Bind data
- Merge test and train data
- Apply mean function to dataset using dcast function
- Create new tidy_data.txt" with avg for each activity and subject
