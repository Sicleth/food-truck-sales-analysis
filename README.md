# 🚚 Food Truck Sales Analysis

End-to-end data analysis project applying real-world data analyst techniques to my own food truck business — from raw sales data to actionable business insights.

## 📌 Objective

This project simulates a real business analytics workflow: collecting, cleaning, analyzing, and visualizing sales data to answer key business questions and support data-driven decision-making for the food truck operation.

## ❓ Business Questions

- What days/times generate the highest revenue?
- Which products have the best margin and turnover (not just top sellers)?
- Is there seasonality in sales (weather, events, time of month)?
- What is the average ticket size, and how does it vary by day/location?
- Which locations (if applicable) are the most profitable?

## 🛠️ Tools & Techniques

| Stage | Tools |
|---|---|
| Data cleaning & wrangling | Python (Pandas) |
| Database & queries | SQL (SQLite) |
| Exploratory analysis | Python (Pandas, Matplotlib) |
| Dashboard & reporting | Power BI / Tableau |

## 📁 Project Structure

```
food-truck-sales-analysis/
│
├── data/
│   ├── raw/                  # Original data (anonymized)
│   └── processed/            # Cleaned data ready for analysis
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   └── 02_exploratory_analysis.ipynb
│
├── sql/
│   ├── schema.sql            # Database structure
│   └── queries.sql           # Business-question queries
│
├── dashboard/
│   └── food_truck_dashboard.pbix   # or .twbx (Tableau)
│
├── reports/
│   └── insights_summary.md   # Key findings & recommendations
│
└── README.md
```

## 🔍 Methodology

1. **Data Collection** — Sales data exported from [source: spreadsheet/POS system].
2. **Data Cleaning** — Handled missing values, duplicates, inconsistent date/time formats, and standardized product categories using Pandas.
3. **Database Modeling** — Structured the data into relational tables (sales, products, dates/locations) in SQLite and wrote SQL queries to answer core business questions.
4. **Exploratory Data Analysis** — Identified trends, seasonality, and patterns using Pandas and Matplotlib.
5. **Dashboard** — Built an interactive dashboard for at-a-glance business monitoring.
6. **Insights & Recommendations** — Translated findings into practical recommendations for the business.

## 📊 Key Insights

*(To be completed after analysis — e.g., best-selling days, most profitable items, revenue trends)*

## 🚀 How to Run This Project

```bash
# Clone the repository
git clone https://github.com/Sicleth/food-truck-sales-analysis.git

# Install dependencies
pip install pandas matplotlib jupyter

# Run notebooks
jupyter notebook notebooks/01_data_cleaning.ipynb
```

## 👤 About Me

This project is part of my portfolio as I pursue a career as a Data Analyst, applying skills from the **IBM Data Analyst Professional Certificate** to a real-world business I run myself.