# Assignment-Getting-and-Cleaning-Data

## Project Overview
This project demonstrates data cleaning techniques by processing and tidying data collected from the accelerometers of Samsung Galaxy S smartphones. The goal is to create a tidy data set that can be used for later analysis.

## Files
- **run_analysis.R**: R script that performs the data cleaning and transformation steps.
- **tidy_dataset.txt**: The final tidy data set with the average of each variable for each activity and subject.
- **CodeBook.md**: Documentation of variables, transformations, and data structure.
- **README.md**: This file, providing an overview and usage instructions.

## Instructions
1. **Download Data**: Run the `run_analysis.R` script, which will automatically download and unzip the dataset if it's not already in the working directory.
2. **Process Data**: The script merges, filters, labels, and calculates averages as described in the project instructions.
3. **Output**: A tidy data set will be created as `tidy_dataset.txt` in the working directory.

## Running the Script
1. Open R or RStudio.
2. Set the working directory to the location of `run_analysis.R`.
3. Run the script:
   ```r
   source("run_analysis.R")
