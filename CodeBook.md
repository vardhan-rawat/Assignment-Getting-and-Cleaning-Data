# Codebook for UCI HAR Dataset - Human Activity Recognition

## Variables

### Subject
- **subject**: Integer representing the ID of the participant.

### Activity
- **activity**: A factor variable representing the activity performed by the participant. The possible values are:
  - WALKING
  - WALKING_UPSTAIRS
  - WALKING_DOWNSTAIRS
  - SITTING
  - STANDING
  - LAYING

### Measurements
The following variables represent measurements of accelerometer and gyroscope data. All variables are collected from sensors and represent different statistical summaries (mean and standard deviation) of the signal data.

- **timeDomainAccMeanX**: Mean value of accelerometer signal in the X direction (time domain).
- **timeDomainAccMeanY**: Mean value of accelerometer signal in the Y direction (time domain).
- **timeDomainAccMeanZ**: Mean value of accelerometer signal in the Z direction (time domain).
- **timeDomainAccStdX**: Standard deviation of accelerometer signal in the X direction (time domain).
- **timeDomainAccStdY**: Standard deviation of accelerometer signal in the Y direction (time domain).
- **timeDomainAccStdZ**: Standard deviation of accelerometer signal in the Z direction (time domain).
- **frequencyDomainAccMeanX**: Mean value of accelerometer signal in the X direction (frequency domain).
- **frequencyDomainAccMeanY**: Mean value of accelerometer signal in the Y direction (frequency domain).
- **frequencyDomainAccMeanZ**: Mean value of accelerometer signal in the Z direction (frequency domain).
- **frequencyDomainAccStdX**: Standard deviation of accelerometer signal in the X direction (frequency domain).
- **frequencyDomainAccStdY**: Standard deviation of accelerometer signal in the Y direction (frequency domain).
- **frequencyDomainAccStdZ**: Standard deviation of accelerometer signal in the Z direction (frequency domain).
- **timeDomainGyroMeanX**: Mean value of gyroscope signal in the X direction (time domain).
- **timeDomainGyroMeanY**: Mean value of gyroscope signal in the Y direction (time domain).
- **timeDomainGyroMeanZ**: Mean value of gyroscope signal in the Z direction (time domain).
- **timeDomainGyroStdX**: Standard deviation of gyroscope signal in the X direction (time domain).
- **timeDomainGyroStdY**: Standard deviation of gyroscope signal in the Y direction (time domain).
- **timeDomainGyroStdZ**: Standard deviation of gyroscope signal in the Z direction (time domain).

## Data Cleaning

- **Special Characters**: The column names are cleaned by removing special characters such as parentheses and dashes.
- **Abbreviations**: Abbreviations are expanded to more descriptive terms, e.g., `Acc` becomes `Accelerometer`, `Gyro` becomes `Gyroscope`.
- **Variable Naming**: All variable names are modified to follow consistent naming conventions. For example, `mean` is capitalized to `Mean` and `std` becomes `StandardDeviation`.

## Summary

This dataset represents sensor readings from 30 participants performing 6 activities. The final tidy dataset includes the mean of each variable for each subject and activity, providing a summary of sensor data across different activities and subjects.
