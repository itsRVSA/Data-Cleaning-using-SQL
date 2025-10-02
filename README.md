# Data-Cleaning-using-SQL
Data Cleaning using SQL 
Data-Cleaning
This project demonstrates a data cleaning workflow for a dataset of company layoffs. The goal is to transform raw, messy data into a clean, standardized dataset ready for analysis. The script works on a raw table (layoffs) and outputs a cleaned staging table (layoff_staging2) while keeping the original data intact.

*Key Features

Data Staging: Creates a safe staging table for data manipulation without affecting the original table.

Removing Duplicates: Uses CTEs and ROW_NUMBER() to identify and remove duplicate rows efficiently.

Standardizing Data: Trims extra spaces, normalizes industry names, cleans country names, and converts string dates to proper DATE format.

Handling Nulls & Blanks: Detects missing critical values, fills missing industry values using existing company records, and removes invalid rows.

Cleanup: Drops temporary helper columns to maintain a clean, analyzable table.

Views for Analysis: Creates a view (high_funded_companies) to easily query top-funded finance companies.

**SQL Concepts Used

CTEs & Window Functions (ROW_NUMBER) → Deduplication

String Functions (TRIM, TRAILING) → Standardizing text

Date Functions (STR_TO_DATE) → Converting dates

Null Handling & Joins → Filling missing values

DROP & DELETE → Removing unnecessary data

Views → Filtered, reusable datasets

Staging Tables → Safe intermediate processing
