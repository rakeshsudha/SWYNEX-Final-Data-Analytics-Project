# SWYNEX Final Data Analytics Project

## Project Overview

This project is the final Data Analytics case study completed as part of my Data Analyst Internship at SWYNEX.

The project combines the complete data analytics workflow, starting from data cleaning and exploratory data analysis and progressing to an interactive Power BI dashboard and business insights.

## Project Objective

The objective of this project is to analyze retail store sales data, identify important trends and patterns, and present the findings through an interactive Power BI dashboard.

## Dataset

The project uses the **Retail Store Sales — Dirty for Data Cleaning** dataset.

The dataset contains information about:

- Transaction ID
- Customer ID
- Category
- Item
- Price Per Unit
- Quantity
- Total Spent
- Payment Method
- Location
- Transaction Date
- Discount Applied

## 1. Data Cleaning

The raw dataset was cleaned using Python and Pandas.

### Data Cleaning Activities

- Identified and handled missing values
- Checked for duplicate records
- Checked duplicate Transaction IDs
- Converted Transaction Date to the correct datetime format
- Checked numeric columns for invalid negative or zero values
- Checked categorical values for consistency
- Reconstructed missing Price Per Unit values where possible
- Filled missing Quantity values using category-level median values
- Recalculated missing Total Spent values using Price Per Unit × Quantity
- Recovered missing Item values using Category and Price Per Unit relationships
- Replaced unavailable Discount Applied values with `Unknown`

### Validation

The cleaned dataset was validated for:

- Missing values
- Duplicate records
- Duplicate Transaction IDs
- Invalid numeric values
- Data type consistency
- Total Spent calculation consistency

## 2. Exploratory Data Analysis

Exploratory Data Analysis was performed using Python, Pandas and visualization libraries.

### Analysis Performed

- Descriptive statistics
- Key business metrics
- Sales by category
- Sales by payment method
- Sales by location
- Monthly sales trends
- Top 10 items by sales
- Discount analysis
- Outlier analysis
- Category transaction analysis
- Sales per transaction by category
- Average transaction value by payment method

## 3. Power BI Dashboard

An interactive Power BI dashboard was developed to communicate the major findings from the analysis.

### Key Performance Indicators

- Total Sales: 1.64M
- Total Transactions: 12,575
- Average Transaction Value: 130.08
- Total Quantity Sold: 69,828

### Dashboard Visualizations

- Sales by Category
- Monthly Sales Trend
- Sales by Payment Method
- Sales by Location
- Top 10 Items by Sales
- Sales by Discount Status

### Interactive Filters

The dashboard includes slicers for:

- Transaction Date
- Category
- Payment Method

## 4. Key Business Insights

- The dataset contains 12,575 transactions with total sales of approximately 1.64M.
- The average transaction value is approximately 130.08, while the median transaction value is 110.00.
- Butchers recorded the highest category-level sales at approximately 216.48K.
- Milk Products recorded the lowest category-level sales at approximately 189.89K.
- Online sales were approximately 831.13K, slightly higher than in-store sales of approximately 804.56K.
- Item_25_FUR generated the highest individual item sales at approximately 27.10K.
- Cash had the highest average transaction value among the payment methods, at approximately 131.50.
- Outlier analysis identified 60 transactions above the upper IQR limit of 402. These were reviewed and were consistent with the Price Per Unit × Quantity relationship.

## 5. Tools and Technologies

- Python
- Pandas
- Matplotlib
- Seaborn
- Power BI
- DAX
- GitHub

## 6. Project Files

- `Data_Cleaning.ipynb` — Data cleaning process
- `Task_2_EDA.ipynb` — Exploratory Data Analysis
- `cleaned_retail_store_sales.csv` — Cleaned dataset
- `Retail_Store_Sales_Dashboard.pbix` — Power BI dashboard
- `dashboard_preview.png` — Dashboard preview

## Dataset Source

Kaggle:

https://www.kaggle.com/datasets/ahmedmohamed2003/retail-store-sales-dirty-for-data-cleaning

## Internship

**Data Analyst Internship — SWYNEX**

## Conclusion

This project demonstrates the complete data analytics workflow from raw data preparation to exploratory analysis, interactive dashboard development, and business insight generation.

The project helped strengthen practical skills in data cleaning, exploratory data analysis, Power BI, DAX, data visualization, and business-focused analytical reporting.
