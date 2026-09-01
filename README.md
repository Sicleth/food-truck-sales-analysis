# 🚚 Food Truck Sales Analysis

End-to-end data analysis project using real sales data from my own food truck business — from raw data cleaning and transformation to SQL analysis, data visualization, and actionable business insights.

The project follows a real-world Data Analyst workflow focused on understanding sales performance, identifying patterns, and supporting data-driven business decisions.

## 📌 Objective

The objective of this project is to analyze historical food truck sales data to understand when sales happen, which products drive revenue, and how sales performance changes over time.

The analysis combines Python, SQL, and Power BI to transform raw operational data into meaningful business insights and recommendations.

## ❓ Business Questions

The analysis focuses on the following business questions:

- Which days of the week generate the highest revenue?
- Which hours generate the highest and lowest revenue?
- Is there a clear growth, decline, or seasonal pattern in revenue?
- How does the average ticket change over time?
- Is there a difference between the products with the highest sales volume and those generating the most revenue?
- How concentrated is revenue among the top-selling products?
- Are there recurring patterns throughout the month that could support operational decisions?

Note: Product profitability was not analyzed because historical product-level cost data was not available in the source data.

## 🛠️ Tools & Techniques

Stage                          |         Tools / Techniques
Data cleaning & transformation |         Python, Pandas
Data modeling & querying	   |         SQL, SQLite
Exploratory Data Analysis	   |         Pandas, Matplotlib
Data visualization	           |         Matplotlib, Power BI
Business intelligence	       |         Power BI, DAX
Development environment        |         Jupyter Notebook
Version control   	           |         Git, GitHub

## 📁 Project Structure

```
food-truck-sales-analysis/
│
├── data/
│   ├── raw/                  # Original data (anonymized)
|   |   ├── kyte/
|   |   ├── manual_spreadsheet/
|   |
│   └── processed/            # Cleaned data ready for analysis
|       ├── items_sold.csv/
|       ├── monthly_expenses.csv/
|       ├── revenue.csv/
|       ├── sales_detail.csv/
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   |── 02_sql_modeling.ipynb
│   └── 03_visualization.ipynb
│
├── sql/
│   └── food_truck.db          
│
├── dashboard/
│   └── food_truck_dashboard.pbix   
│
│
└── README.md
```

## 🔍 Methodology

1. Data Collection

Sales data was collected from the food truck's operational records, including exported sales data and manually maintained spreadsheets.

2. Data Cleaning & Transformation

Python and Pandas were used to prepare the raw data for analysis.

The process included:

- handling missing values;
- identifying and removing duplicated records;
- standardizing date and time fields;
- transforming data types;
- cleaning product names and categories;
- creating structured datasets for analysis.

3. SQL Analysis

The cleaned data was structured and analyzed using SQLite.

SQL queries were used to answer business questions related to:

- revenue;
- sales volume;
- product performance;
- time-based patterns;
- orders and average ticket.

4. Exploratory Data Analysis

Pandas and Matplotlib were used to explore trends and patterns before building the final dashboard.

The exploratory analysis focused on:

- revenue trends;
- weekday performance;
- hourly sales patterns;
- average ticket;
- product sales volume;
- product revenue contribution.

5. Power BI Dashboard

An interactive Power BI dashboard was created with three analytical perspectives:

Executive Overview

Provides a high-level view of:

Total Revenue
Total Orders
Average Ticket
Total Units Sold
Revenue Over Time
Revenue by Weekday
Estimated Revenue by Product
Sales Performance

Focuses on temporal sales patterns:

Revenue by Day of Month
Orders by Weekday
Average Ticket Trend
Revenue by Month
Weekly Revenue Trend
Revenue by Hour
Product Analysis

Focuses on product performance:

Top Products by Revenue
Top Products by Quantity
Revenue Contribution by Product

## 📊 Key Insights

The insights below follow a consistent analytical structure:

Observation → Why it matters → Recommendation

1. [Strongest Revenue Day]

Observation: Saturday generated the highest total revenue, with   R$172.496,00, representing approximately 25% of total revenue.

Why it matters: The strongest weekday represents a significant portion of the business's sales performance and should receive greater operational attention.

Recommendation: Prioritize stock preparation and operational capacity on Saturday, ensuring the most frequently sold products are available during the highest-demand periods.

2. [Afternoon Sales Peak]

Observation: Revenue reaches its highest level around 16:00, while the lowest revenue period occurs around 13:00 and 19:00.

Why it matters: Sales are concentrated during specific hours, meaning operational resources are not equally valuable throughout the entire working period.

Recommendation: Increase inventory and preparation capacity before the afternoon peak and evaluate whether low-demand hours justify the same operating capacity.

3. [Revenue Trend / Seasonality]

Observation: Monthly revenue reached its highest level in December, while the lowest recorded month was June.

Why it matters: The difference between stronger and weaker periods indicates that sales performance varies significantly over time rather than remaining constant.

Recommendation: Use historical performance to plan inventory and operating capacity ahead of stronger periods and investigate the causes of unusually weak months.

4. [Average Ticket Pattern]

Observation: The average ticket changed from approximately R$ 13 to  R$18 during the analyzed period.

Why it matters: Changes in average ticket indicate whether revenue changes are being driven mainly by the number of orders or by the amount spent per order.

Recommendation: Monitor average ticket alongside order volume when evaluating future pricing or product-bundling strategies.

5. [Volume vs Revenue]

Observation: 'Casquinha' ranks highly in sales volume and also generates higher estimated revenue.

Why it matters: In this case the top sales product is the product with the highest revenue as well, but isn't necessarily always true.

Recommendation: Use both sales volume and estimated revenue when evaluating product performance rather than relying only on the number of units sold.

6. [Revenue Concentration]

Observation: The top three products account for 50% of estimated total revenue.

Why it matters: A high concentration means overall revenue depends heavily on a relatively small number of products.

Recommendation: Prioritize availability of the leading products while monitoring the performance of lower-contributing products to identify opportunities for assortment or pricing adjustments.

⚠️ Data Limitations

This analysis has some important limitations that should be considered when interpreting the results.

Estimated Product Revenue

Historical product-level prices were not consistently available in the source data. Therefore, product revenue is estimated using current menu prices.

Product Costs

Historical product-level cost data was not available. As a result, this project does not calculate actual product-level profit margins or profitability.

Item-Level Dates

Product-level historical timestamps were not available for all records. Therefore, some time-based product analyses are limited.

These limitations are explicitly documented to avoid presenting estimates as historical financial results.

💡 Business Recommendations

Based on the analysis, the main opportunities identified are:

align inventory preparation with peak sales hours;
monitor weekday and monthly revenue patterns when planning operations;
prioritize high-revenue and high-volume products for stock availability;
monitor average ticket together with order volume;
investigate unusually strong or weak periods to understand the operational or external factors behind them;
incorporate historical product costs in future analyses to enable actual margin and profitability analysis.

## 🚀 How to Run This Project

```bash
# Clone the repository
git clone https://github.com/Sicleth/food-truck-sales-analysis.git cd food-truck-sales-analysis

# Install dependencies
pip install pandas matplotlib jupyter

# Run notebooks
jupyter notebook

Then open the notebooks in the following order:

01_data_cleaning.ipynb
02_sql_modeling.ipynb
03_visualization.ipynb
```

## 👤 About Me

This project is part of my portfolio as I transition into a career in Data Analytics.

I developed this project using real data from a business I operate myself, applying skills developed through the IBM Data Analyst Professional Certificate and independent study.

The goal was not only to practice technical tools, but to demonstrate how data can be transformed into insights that support real business decisions.

Tools used: Python • Pandas • SQL • SQLite • Matplotlib • Power BI • Jupyter Notebook • Git • GitHub