SQL Data Cleaning – Nashville Housing Project

Project Overview

This project focuses on cleaning and transforming raw housing data using SQL Server. The dataset contains real estate records from Nashville, requiring extensive cleaning for accurate analysis and reporting. The key objectives include standardizing formats, handling missing values, and optimizing data structure. By performing data cleaning, we ensure accuracy, consistency, and efficiency, making the dataset more reliable for further analysis and visualization.

Dataset

Source: Nashville Housing Data

Database: SQL Server

Table: NashvilleHousing

Cleaning Steps & SQL Queries

1. Standardizing Date Format

Converted SaleDate to a standard DATE format.

Created a new column SaleDateConverted and updated records.

2. Handling Missing Property Address

Used self-join to populate missing property addresses based on matching ParcelID.

3. Splitting Address into Components

Extracted Street Address and City from PropertyAddress.

Split OwnerAddress into OwnerStreet, OwnerCity, and OwnerState using PARSENAME().

4. Standardizing "Sold As Vacant" Field

Replaced Y and N values with Yes and No for better readability.

5. Removing Duplicates

Identified duplicate records using ROW_NUMBER() and removed them.

6. Dropping Unused Columns

Removed unnecessary fields (OwnerAddress, TaxDistrict, PropertyAddress, SaleDate) to improve efficiency.

SQL Techniques Used

✅ Data Type Conversion

✅ String Functions (SUBSTRING, CHARINDEX, PARSENAME)

✅ Conditional Updates (CASE WHEN)

✅ Joins (Self-Join)

✅ CTE & Window Functions (ROW_NUMBER())

✅ ALTER TABLE (Adding/Dropping Columns)

Future Enhancements

🔹 Further data normalization to improve consistency and efficiency.

🔹 Automating the cleaning process with stored procedures.

🔹 Visualizing the cleaned data using Power BI/Tableau for better insights.

By refining and structuring the data effectively, this project enhances data quality and prepares it for deeper analysis and reporting. The goal is to make the dataset more actionable and insightful for decision-making. 🚀
