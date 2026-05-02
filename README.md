# NIke-sales-dataset
# 📊 Nike Sales Data Analysis (Excel + Power BI)

## 🔍 Project Overview

This project focuses on analyzing an uncleaned Nike sales dataset to extract meaningful business insights. The dataset contained multiple inconsistencies such as missing values, mixed data formats, and incorrect entries, which were systematically cleaned and transformed before analysis.

---

## 🧹 Data Cleaning & Transformation

### 1. Handling Missing Values

* Identified missing values in critical columns such as **Units Sold, MRP, Discount, and Order Date**
* Applied:

  * Product-based averaging for Units and MRP using conditional aggregation
  * Category-based averaging for Discount
  * Forward-fill technique for missing dates
* Removed rows where multiple critical fields were missing to maintain data reliability


2. Standardizing Size Data
•	Dataset contained mixed size formats (numeric + text in wrong categories)
•	Created:
o	Product_Type (Shoe vs Clothing)
o	Size_Type (Numeric vs Text)
•	Built a standardized Final_Size column:
o	Clothing → restricted to S, M, L, XL
o	Shoes → restricted to numeric sizes
•	Applied default values where inconsistencies were detected
________________________________________


3. Date Cleaning & Formatting
•	Resolved inconsistent formats (DD/MM/YYYY vs DD-MM-YYYY)
•	Converted text dates into proper date format
•	Filled missing dates using forward-fill logic
•	Extracted Month and Year for time-based analysis
________________________________________


 4. Revenue & Profit Validation
•	Recalculated revenue using:
o	Units × MRP × (1 - Discount)
•	Identified and flagged:
o	Zero revenue with non-zero units
o	Negative or inconsistent profit values
________________________________________

5. Data Standardization
•	Cleaned categorical inconsistencies:
o	Region names (e.g., Hyd → Hyderabad)
o	Product naming inconsistencies
•	Ensured uniform formatting across dataset
________________________________________
6. Data Validation Checks
•	Ensured:
o	Units are integers (no decimal sales)
o	Discount values lie between 0–1
o	No duplicate records
o	Outliers identified and reviewed
________________________________________

## Live Dashboard
View pivot tables and analysis here:
[Nike Sales Dashboard](https://docs.google.com/spreadsheets/d/1emqXnNPDODYUVR5vKcpzCfnnEexYuTf_ascGmv0gfBM/edit?gid=1757264485#gid=1757264485)

