# OIBSIP
# Data Analytics Track — Task 3: Cleaning Data

## Objective
Clean a messy employee dataset (1,020 rows) into an analysis-ready dataset, 
documenting every cleaning decision made.

## Dataset
- Source: Kaggle (messy employee dataset)
- Original file: Messy_Employee_dataset.csv
- Cleaned file: Messy_Employee_dataset_cleaned.csv

## Data Quality Report (Before Cleaning)
- Missing values: Age (211), Salary (24)
- Duplicate rows: 0
- Data type issues: Join_Date stored as text, Phone stored as negative integers,
  Department_Region combined into a single column

## Cleaning Steps Performed
1. **Missing data handling**: Age and Salary missing values filled using median 
   (robust to outliers, appropriate for skewed numeric data). Rows were not 
   dropped since Age was missing in ~21% of rows — too significant to discard.
2. **Duplicate removal**: Checked using `.duplicated()` — 0 duplicates found.
3. **Standardisation**: Verified Status, Performance_Score, and Remote_Work 
   columns using `.unique()` — no inconsistent formatting found.
4. **Outlier detection**: Applied IQR method (1.5× multiplier) to Age and 
   Salary — 0 outliers found in either column.
5. **Data type correction**: Converted Join_Date to datetime, Phone to string.
6. **Column split**: Split Department_Region into separate Department and 
   Region columns; dropped the original combined column.

## Before vs. After Summary
| Metric | Before Cleaning | After Cleaning |
|---|---|---|
| Total rows | 1,020 | 1,020 |
| Total columns | 12 | 13 (Department_Region split into Department + Region) |
| Missing values — Age | 211 | 0 (filled with median) |
| Missing values — Salary | 24 | 0 (filled with median) |
| Duplicate rows | 0 | 0 |
| Join_Date dtype | object (string) | datetime64 |
| Phone dtype | int64 (negative values) | string |
| Salary outliers (IQR method) | Not checked | 0 found |
| Age outliers (IQR method) | Not checked | 0 found |
| Category formatting | Unchecked | Verified clean |

## Tools Used
Python, pandas, Jupyter Notebook
