# Task 1: Data Cleaning and Preprocessing

## Project Overview
This project focuses on cleaning and preprocessing the Customer Personality Analysis dataset using Python and Pandas.

The objective was to identify and handle missing values, duplicates, outliers, inconsistent categorical values, and incorrect data types.

## Tools Used
- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

## Dataset
Customer Personality Analysis – Marketing Campaign Dataset.

Original dataset: `dataset/marketing_campaign.csv`

## Data Cleaning Steps

1. **Missing Values**
   - Identified 24 missing values in the Income column.
   - Replaced them using the median Income value (51,381.5).

2. **Duplicate Records**
   - Checked for duplicate rows.
   - Checked for duplicate customer IDs.
   - No duplicates were found.

3. **Outlier Detection**
   - Used the Interquartile Range (IQR) method.
   - Identified 8 potential Income outliers.
   - Retained these values because there was insufficient evidence to classify them as errors.

4. **Categorical Data Cleaning**
   - Inspected Education and Marital_Status.
   - Replaced invalid categories 'Absurd' and 'YOLO' with missing values.
   - Retained the 'Alone' category.
   - Removed unnecessary leading and trailing whitespace.

5. **Date Conversion**
   - Converted Dt_Customer into datetime format.

6. **Column Name Standardization**
   - Converted column names to lowercase.
   - Removed leading and trailing whitespace from column names.

7. **Data Type Verification**
   - Verified numerical and categorical data types.

## Final Dataset
- Total records: 2,240
- Total columns: 29
- Missing Income values: 0
- Missing Marital_Status values: 4
- Duplicate records: 0
- Duplicate customer IDs: 0

## Project Structure
- `dataset/`: Original dataset.
- `cleaned_data/`: Cleaned CSV dataset.
- `notebooks/`: Jupyter Notebook containing the cleaning process.
- `README.md`: Project documentation.

## Conclusion
The dataset was cleaned and prepared for further analysis. Missing values, categorical inconsistencies, date formats, and data types were addressed. Potential outliers were retained after identification and inspection.

The resulting dataset is ready for further exploratory data analysis.