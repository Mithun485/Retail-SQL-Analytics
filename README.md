
# Retail SQL Analytics Project

A complete end-to-end SQL analytics system designed to demonstrate real Data Analyst skills, including data modeling, KPI creation, advanced SQL, trend forecasting, seasonality, Pareto analysis, and data quality validation.

---

# Project Overview

This project analyzes Retail sales data using SQL Server.


---

# Project Structure

```
Retail-SQL-Analytics/
│
├── data/
│   └── sales_data.csv
│
├── sql/
│   ├── create_tables.sql
│   ├── insert_data.sql
│   ├── analytics_queries.sql
│   ├── insights_queries.sql
│   ├── data_quality_checks.sql
│   └── advanced_queries.sql
│
└── notes/
    └── project_notes.txt


# 🛠Tech Stack

* SQL Server
* CTEs, Window Functions
* Aggregations, Joins, Subqueries
* Date/Time functions
* Statistical SQL functions (REGR_SLOPE, REGR_INTERCEPT)
* Data Quality Validation Techniques



# 📂 Dataset Description

The dataset contains synthetic retail sales data with:

Tables

| Table      | Description                            |
| ---------- | -------------------------------------- |
|  sales     | Individual daily sales transactions    |
|  products  | Product master data (category, vendor) |
|  vendors   | Vendor-level information               |

### **Fields Included**

* sale_id
* product_id
* sale_date
* quantity
* unit_price
* vendor_id
* category

The data was artificially generated to simulate realistic variations such as seasonality, vendor performance differences, and varying unit prices.


---

# Key Business Questions Answered

### 1. Revenue & Volume Trends

* Total revenue
* Average order value
* Best-selling products
* Revenue by category
* Top-performing vendors

### 2. Seasonality

* Monthly revenue pattern
* Beverage seasonality (summer spikes)
* Trend comparison across months & categories

### 3. Year-over-Year & Month-over-Month Trends

* Revenue growth
* Product-level growth
* Vendor-level contribution changes

### 4. Forecasting (SQL-Based Linear Regression)

Using `REGR_SLOPE` and `REGR_INTERCEPT`, the project predicts expected revenue based on historical trend data.

### 5. Pareto Analysis (80/20 Rule)

Identifies which products contribute most of the revenue.

---

# Advanced Analytics Included

### Pareto 80/20 Analysis

Determines whether 20% of products generate 80% of revenue.

The 20% generating 80% profit means they are your segment making more profit in the business - it doesn't mean to neglect other - it is just to find the top segment while making decision's.



### Price Elasticity of Demand (Simulated)

SQL logic used to estimate customer sensitivity to price changes.

Here the data set didn't have the actual A/B test data so we simulated the elasticity to give idea on the price elasticity concept.

> Includes a full disclaimer:
> real elasticity analysis requires actual price variations or A/B testing.

### Linear Forecasting

Predicts revenue trend using regression functions:

* REGR_SLOPE
* REGR_INTERCEPT

Creates a clean forward-looking revenue projection.

This is the linear model - and parameters wont consider outside factors
---

# Data Quality Checks (DQC)

data validation is included in the data_quality.sql file-

* Missing values
* Orphan keys (broken joins)
* Duplicate sales
* Negative/invalid quantities or prices
* Outlier detection (Z-score)
* Logical inconsistencies
* Category/vendor mismatches

These checks mirror what real analysts and data engineers perform before running analytics.

---

# Example KPIs Calculated

* Total Revenue
* Average Revenue Per Day
* Average Order Value (AOV)
* Top 5 Grossing Products
* Revenue by Category
* Vendor Contribution %
* Monthly Revenue Trend
* YOY Revenue Change
* Rolling 3-Month Average Revenue
* Top 10 Highest Revenue Days

All KPIs are written in SQL with clean formatting and comments.


# 📈 Sample Insights (Business-Focused)

* Beverages show clear seasonality, with increased sales in warmer months.
* Top 3 products contribute the majority of revenue, confirming a Pareto distribution.
* Vendor B consistently outperforms others, indicating strong partnerships.
* Forecasting shows an upward revenue trend, suggesting healthy business growth.
* Data quality checks identified no major structural issues, validating dataset reliability.

---

▶️ How to Run the Project

1. Clone the repository
2. Open files in SQL Server
3. Run create_tables.sql
4. Run insert_data.sql
5. Execute query files in this order:

 analytics_queries.sql
 insights_queries.sql
 data_quality_checks.sql
 advanced_queries.sql

---

🙌Author

Mithun Vennapusa
Aspiring Data Analyst / Data Engineer
Focused on SQL, ETL pipelines, business insights, and data modeling.

