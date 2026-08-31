
# Data Analytics Level 1 - Task 3: Data Cleaning

## Project Overview

This project focuses on identifying and correcting data quality issues in a large Titanic passenger dataset.

The cleaning process includes missing-value handling, duplicate checking, data standardization, outlier detection, data type correction, and validation of the final cleaned dataset.

## Dataset

The dataset contains 1,000,000 Titanic passenger records and 12 columns.

Important columns include:

- PassengerId
- Survived
- Pclass
- Name
- Sex
- Age
- SibSp
- Parch
- Ticket
- Fare
- Cabin
- Embarked

## Data Quality Issues Identified

The initial inspection identified:

- 198,600 missing values in `Age`
- 770,195 missing values in `Cabin`
- 2,240 missing values in `Embarked`
- 0 duplicate rows

## Data Cleaning Process

### Missing Values

- `Age` missing values were replaced using the median.
- `Cabin` missing values were replaced with `Unknown`.
- `Embarked` missing values were replaced using the mode.

### Duplicate Records

Duplicate records were checked and no duplicates were found.

### Data Standardization

Categorical values and column names were standardized to maintain consistency.

### Outlier Handling

Potential outliers in `Age` and `Fare` were identified using the IQR method.

Instead of deleting records, extreme values were capped at the IQR boundaries to preserve the dataset.

### Data Type Correction

Numerical and categorical columns were converted to appropriate data types.

## Before vs After Cleaning

| Metric | Before Cleaning | After Cleaning |
|---|---:|---:|
| Number of Rows | 1,000,000 | 1,000,000 |
| Number of Columns | 12 | 12 |
| Missing Values | 971,035 | 0 |
| Duplicate Rows | 0 | 0 |

## Final Result

After cleaning, the dataset contains:

- 1,000,000 rows
- 12 columns
- 0 missing values
- 0 duplicate rows

The cleaned dataset was exported as:

`cleaned_titanic_dataset.csv`

## Conclusion

The data cleaning process successfully improved the quality and consistency of the Titanic dataset. The final dataset is ready for further analysis and machine learning applications.
