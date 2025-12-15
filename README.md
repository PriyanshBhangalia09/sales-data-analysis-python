# Sales Data Cleaning & Analysis using Python

This project demonstrates an end-to-end data analysis workflow on an e-commerce sales dataset using Python.  
The focus is on data cleaning, validation, feature engineering, and exploratory data analysis (EDA) to extract business insights.

---

## 📌 Project Objectives
- Clean and validate raw sales data
- Handle duplicate transactional records correctly
- Engineer business-relevant features and KPIs
- Perform exploratory data analysis to identify trends and patterns
- Prepare an analysis-ready dataset for SQL and BI tools

---

## 🛠️ Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib

---

## 📂 Dataset
- Retail e-commerce (Superstore-style) sales dataset
- ~10,000 transaction records
- Contains order, customer, product, sales, discount, and profit details

---

## 🔄 Workflow Overview

### 1. Data Loading & Initial Exploration (EDA – Part 1)
- Loaded CSV data using Pandas
- Inspected dataset structure, columns, data types, and numeric ranges

### 2. Data Cleaning & Preparation
- Standardized column names
- Removed non-informative columns
- Converted date columns to datetime format

### 3. Data Validation & Duplicate Handling
- Checked for missing values
- Identified duplicate order–product records
- Removed true duplicates
- Aggregated split line items to ensure one row per order–product–discount

### 4. Feature Engineering
- Renamed sales to revenue
- Created time-based features (year, month, year-month)
- Calculated shipping duration
- Derived profit margin

### 5. Business KPIs
- Total Revenue
- Total Profit
- Total Orders

### 6. Exploratory Data Analysis (EDA – Part 2)
- Monthly revenue trend analysis
- Top products by revenue
- Revenue by category
- Discount vs profit analysis

### 7. Output & Pipeline Support
- Exported final cleaned dataset for downstream SQL and BI analysis

---

## 📊 Key Insights
- Revenue shows seasonal variation with an overall upward trend
- A small set of products contributes a significant share of total revenue
- High discounts do not consistently lead to higher profits
- Some orders operate at negative profit margins

---

## 📁 Repository Contents
- `sales_data_analysis.ipynb` – Jupyter Notebook containing full analysis
- `superstore_final_clean.csv` – Cleaned, analysis-ready dataset
- `README.md` – Project documentation

---

## 🚀 How to Run
1. Clone the repository
2. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib
