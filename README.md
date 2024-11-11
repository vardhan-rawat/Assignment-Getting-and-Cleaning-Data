# UCI HAR Dataset - Human Activity Recognition

This repository contains an analysis of the UCI Human Activity Recognition dataset, focusing on the processing, transformation, and summarization of data to create a clean, tidy dataset suitable for analysis.

## Dataset Description

The UCI Human Activity Recognition (HAR) dataset contains sensor data collected from 30 participants performing various physical activities, including walking, walking upstairs, walking downstairs, sitting, standing, and laying. The dataset includes:

- **subject_train.txt**: IDs of participants for the training dataset.
- **X_train.txt**: Training data containing sensor readings from the accelerometer and gyroscope.
- **y_train.txt**: Labels for the training activities.
- **subject_test.txt**: IDs of participants for the test dataset.
- **X_test.txt**: Test data containing sensor readings from the accelerometer and gyroscope.
- **y_test.txt**: Labels for the test activities.
- **features.txt**: List of feature names corresponding to the columns in the training and test data.
- **activity_labels.txt**: Mapping of activity IDs to activity names.

## Steps Taken in the Analysis

1. **Download and Extract Data**: The dataset is downloaded from a URL and unzipped into the working directory.
2. **Data Merging**: The training and test datasets are merged into one data frame.
3. **Extracting Relevant Data**: Columns containing mean and standard deviation values for each measurement are selected.
4. **Descriptive Activity Labels**: Activity labels are converted to descriptive activity names.
5. **Descriptive Variable Names**: The variable names are cleaned and expanded for clarity.
6. **Summarizing Data**: A tidy dataset is created by calculating the average of each variable for each activity and subject.

## Final Output

The output of the analysis is a tidy data file (`tidy_data_cleaned.txt`), which contains the following columns:
- **subject**: ID of the participant.
- **activity**: Descriptive label of the activity performed.
- **Other columns**: Various sensor measurements, including accelerometer and gyroscope data, with descriptive names.

## Running the Analysis

To run the analysis, you need to have the required R packages installed, particularly `dplyr`. After that, execute the provided R script, which will automatically download, process, and create the tidy dataset.

The final clean data is saved as `tidy_data_cleaned.txt`.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
