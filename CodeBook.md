# CodeBook

## Overview
This code book describes the variables, data, and transformations used to create the tidy data set from the "Human Activity Recognition Using Smartphones" dataset.

### Source Data
- Original data collected from accelerometers from Samsung Galaxy S smartphones.
- Available from the UCI Machine Learning Repository: [Link to Dataset](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)

## Variables
- **subject**: Identifier for the subject who performed the activity (integer)
- **activity**: Activity performed by the subject (factor with levels: WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING)
  
### Extracted Features
The following features were extracted for mean and standard deviation measurements:
- timeBodyAcc-mean()-X
- timeBodyAcc-mean()-Y
- timeBodyAcc-mean()-Z
- timeBodyAcc-std()-X
- timeBodyAcc-std()-Y
- timeBodyAcc-std()-Z
- (Continue listing all variables in similar fashion...)

### Transformations
1. **Merged Training and Test Sets**: Combined data from `train` and `test` sets.
2. **Extracted Mean and Standard Deviation Measurements**: Selected only measurements that were means or standard deviations.
3. **Applied Descriptive Activity Names**: Replaced activity IDs with descriptive names.
4. **Labeled Variables**: Updated variable names for clarity.
5. **Created Tidy Data Set**: Generated averages of each variable for each activity and subject, resulting in a tidy dataset.
