# Customer Shopping Behavior Analysis

Analysis of a customer shopping dataset using `Python`, `MySQL`, and `Power BI`.

## Project Overview

This project works with a dataset of 3,900 customer shopping records to examine:

- revenue by customer group
- category performance
- subscription behavior
- discount usage
- customer segmentation

The workflow is:

1. Clean and transform the raw CSV in Python
2. Load the cleaned data into MySQL
3. Answer business questions with SQL
4. Present insights in Power BI
5. Summarize the analysis in the project report

## Dataset

- Source file: [customer_shopping_behavior.csv](customer_shopping_behavior.csv)
- Rows: `3,900`
- Columns: `18`

Main fields include:

- customer demographics: age, gender, location, subscription status
- purchase details: item purchased, category, purchase amount, season, size, color
- behavior fields: previous purchases, frequency of purchases, review rating
- transaction attributes: shipping type, discount applied, payment method


## Data Preparation

The Python notebook includes:

- missing value handling for `Review Rating`
- column renaming to snake case
- creation of `age_group`
- creation of `purchase_frequency_days`
- removal of redundant `promo_code_used`
- export of the cleaned table to MySQL

## SQL Analysis

The SQL script answers questions such as:

- revenue by gender
- customers using discounts with above-average spend
- top-rated products
- subscription vs non-subscription spending
- discount-heavy products
- customer segmentation by previous purchases
- top products within each category
- revenue by age group

## Dashboard

The Power BI dashboard includes:

- customer count
- average purchase amount
- average review rating
- revenue by category
- sales by category
- revenue by age group
- sales by age group
- filters for subscription status, gender, category, and shipping type

## Report

- Summary report: [report.pdf](report.pdf)
- The report consolidates the main findings, business implications, and recommended actions from the analysis.

## Tools Used

- Python: `pandas`, `SQLAlchemy`, `PyMySQL`
- SQL: `MySQL`
- Visualization: `Power BI`
