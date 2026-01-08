# Sales Business Analytics Project

## 📌 Project Overview
This project analyzes the sales performance of a retail superstore using historical transaction data. The goal is to answer key business questions related to revenue, profitability, product performance, customer segments, regions, and the impact of discounts.

## 📊 Business Problem
The business wants to understand how sales and profit are performing over time, which products and segments drive revenue and profitability, where losses occur, and what insights can help improve strategic decisions.

## 🎯 Key Business Questions
1. How have sales and profit trended over time (monthly and yearly)?
2. Which products and categories generate high revenue but low profit?
3. Which regions and customer segments underperform?
4. How do discounts affect profitability?
5. What are the key areas for improvement to maximize profit?

## 📦 Dataset
We use the *Superstore* sales dataset containing order transactions with attributes like sales, profit, discount, region, customer, product information, and dates.  
Download source:  
- Original Kaggle dataset link: https://www.kaggle.com/datasets/vivek468/superstore-dataset-final

## 📁 Project Folder Structure
Sales_Business_Analytics/
│
├── Data/
│ ├── Raw/ # Original dataset
│ └── Clean/ # Cleaned dataset used for analysis
│
├── SQL/
│ ├── sanity_checks.sql # Data validation & integrity checks
│ └── business_queries.sql# Business-focused SQL analysis
│
├── PowerBI/
│ └── Sales_Analytics_Dashboard.pbix
│
├── Images/
│ ├── dashboard_preview.png
│ └── Key_Insights_tooltip.png
│
└── README.md


## 🛠 Tools & Technologies
- Microsoft Excel — Data understanding & cleaning  
- SQL — Structured queries & business metrics  
- Python — Exploratory Data Analysis and deeper insights  
- Power BI — Interactive dashboards


🔹 Data Overview

Dataset contains 9994 rows and 24 columns

Covers sales data from 01/02/2014 to 30/09/2017

Includes orders, products, customers, regions, and financial metrics


### 🔹 Column Review & Decisions
All original columns from the dataset were retained during the cleaning phase to preserve full business context.  
Columns such as `row_id`, `postal_code`, and `country` may not be used directly in analysis but were kept intentionally to maintain data completeness and allow flexibility during later analytical stages.

## Data Cleaning Summary
- Standardized column names for SQL and BI compatibility  
- Verified absence of missing values in key identifier and numeric columns  
- Reviewed duplicate records without removal to preserve transactional integrity  
- Corrected date interpretation to US (MDY) format  
- Created derived date columns (year, month, month number) for time-based analysis  


## 🔍 SQL Analysis & Sanity Checks

SQL was used to validate data integrity and ensure analytical correctness before building the dashboard.

### Sanity Checks Performed
- Verified total row count (9994 rows)
- Validated order date range (2014–2017)
- Checked for NULL values in critical columns (order_id, order_date, sales, profit)
- Confirmed overall totals for sales, profit, and quantity
- Identified loss-making transactions

All validation queries are documented in `sanity_checks.sql`.

### Business Queries (SQL)
SQL queries were written to answer core business questions:
- Year-wise sales and profit trends
- Category-wise revenue and profitability
- Top-performing products by sales
- Identification of loss-making products
- Region-wise performance comparison

These queries helped define the metrics and visuals used in Power BI.

---

## 📊 Power BI Dashboard Overview

An interactive Power BI dashboard was built to present insights in a business-friendly and decision-oriented format.

### Dashboard Features
- KPI Cards:
  - Total Sales
  - Total Profit
  - Total Quantity Sold
- Sales & Profit Trend by Year
- Category-wise Sales and Profit comparison
- Top 10 Products by Sales
- Top 10 Loss-Making Products
- Interactive slicers:
  - Year
  - Region
  - Category
- Custom tooltips for deeper insights on hover

---

## 📈 Key Insights

- **Total Sales:** 2.30M  
- **Total Profit:** 286.40K  
- **Total Quantity Sold:** 38K  

### Business Insights
- Sales and profit show a consistent upward trend from 2014 to 2017
- Technology is the highest revenue-generating category
- Several products generate losses despite having reasonable sales
- High discount levels are closely associated with negative profitability

---

## 🧠 Business Recommendations

- Re-evaluate discount strategies for loss-making products
- Optimize pricing for high-sales but low-profit items
- Focus growth efforts on profitable categories while improving margins
- Investigate underperforming regions and customer segments

---

## 🎯 Project Outcome

This project demonstrates:
- End-to-end analytical thinking
- Strong SQL fundamentals for validation and analysis
- Ability to design interactive, business-focused Power BI dashboards
- Clear translation of data into actionable insights

---

## 🚀 Future Enhancements

- Direct PostgreSQL to Power BI live connection
- Customer segmentation and retention analysis using Python
- Advanced forecasting and profitability modeling

