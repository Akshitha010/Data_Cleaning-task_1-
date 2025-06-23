# Netflix Movies and TV Shows: Data Cleaning and Preprocessing

## Overview

This repository contains the cleaned version of the Netflix Movies and TV Shows dataset, along with the Python code used for data cleaning and a summary of the changes made. The original dataset contained missing values, duplicate records, inconsistent text formats, and non-uniform date formats. The goal was to transform the raw data into a clean, analysis-ready format.

## Cleaning Steps Performed

- **Missing Values:**  
  - Replaced missing values in numeric columns (e.g., `release_year`) with the median of the column.
  - Replaced missing values in text columns (e.g., `director`, `cast`, `country`, etc.) with `"Unknown"`.

- **Duplicates:**  
  - Removed duplicate rows to ensure each entry is unique.

- **Standardization:**  
  - Standardized text columns such as `type`, `country`, `rating`, and `listed_in` to title case and stripped extra spaces.
  - Cleaned `director` and `cast` columns by removing leading/trailing spaces.

- **Date Formatting:**  
  - Converted the `date_added` column to a consistent datetime format.

- **Column Naming:**  
  - Renamed all column headers to lowercase with underscores for consistency.

- **Data Types:**  
  - Ensured `release_year` is stored as an integer.
  - Extracted numeric duration into a new column `duration_int` for easier analysis.

## Files Included

- `netflix_titles.xlsx` - The initial dataset.
- `cleaned_data.xlsx` – The cleaned and processed dataset.
- `Data_Cleaning(task_1).ipynb` – Jupyter Notebook with all cleaning steps and explanations.
- `README.md` – This summary and documentation.

## How to Use

1. Open the Jupyter Notebook to review the cleaning process.
2. The cleaned dataset (`cleaned_data.csv`) is ready for analysis or modeling.

## Learning Outcomes

By completing this task, I gained practical experience in:
- Identifying and handling missing values and duplicates.
- Standardizing and formatting data for consistency.
- Using Pandas for real-world data cleaning tasks.
- Preparing a dataset for further analysis or visualization.

---
