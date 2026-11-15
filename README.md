# 📊 Retail Sales & Business Performance Dashboard

## 📌 Project Overview
This project focuses on analyzing retail sales data using **Microsoft Power BI** to understand business performance, identify sales trends, and generate meaningful business insights.

An interactive dashboard was developed to monitor key performance indicators (KPIs), compare product categories, analyze regional sales, and understand customer payment preferences.

## 🎯 Project Objectives
- Analyze overall sales and profit performance.
- Identify the highest- and lowest-performing product categories.
- Compare sales across different regions.
- Analyze monthly sales trends.
- Identify the top-selling products.
- Understand customer payment preferences.
- Build an interactive dashboard using slicers.

## 🛠️ Tools & Technologies
- Microsoft Power BI
- Power Query
- DAX (Data Analysis Expressions)
- Data Visualization

## 📂 Dataset Information
- Dataset: Retail Sales Dataset
- Records: 100 rows
- Data Format: CSV
- Data Type: Sample/Fictional Retail Data

### Dataset Columns
- Order ID
- Order Date
- Customer Name
- City
- Region
- Category
- Subcategory
- Product
- Quantity
- Unit Price
- Discount Percentage
- Sales
- Total Cost
- Profit
- Payment Mode

## 📈 Dashboard Features

### 1. Key Performance Indicators (KPIs)
- Total Sales
- Total Profit
- Total Orders
- Profit Margin
- Average Order Value (AOV)
- Total Quantity

### 2. Sales Analysis
- Sales by Product Category
- Sales by Region
- Monthly Sales Trend
- Top 5 Products by Sales
- Sales by Payment Mode

### 3. Interactive Filters
- Region Slicer
- Category Slicer

Users can interact with the slicers to explore different segments of the business.

## 🔍 Key Business Insights

Based on the dashboard analysis:

1. **Product Category:** Electronics recorded the highest sales, while Stationery recorded the lowest.
2. **Regional Performance:** East was the highest-performing region, while West recorded the lowest sales.
3. **Monthly Trend:** May recorded the highest sales, while July recorded the lowest.
4. **Product Performance:** Laptop was the top-selling product.
5. **Payment Analysis:** Cash contributed the highest sales, while Net Banking contributed the lowest.

## 🧹 Data Preparation
The dataset was prepared using Power Query:
- Checked for duplicate records.
- Checked for missing values.
- Corrected data types.
- Prepared numerical and categorical columns for analysis.

## 🧮 DAX Measures

Some of the DAX measures used in this project:

```dax
Total Sales = SUM('Sales'[Sales])

Total Profit = SUM('Sales'[Profit])

Total Orders = DISTINCTCOUNT('Sales'[Order_ID])

Total Quantity = SUM('Sales'[Quantity])

AOV = DIVIDE([Total Sales], [Total Orders], 0)

Profit Margin = DIVIDE([Total Profit], [Total Sales], 0)
```

*Note: Replace `'Sales'` with your actual Power BI table name if different.*

## 💡 Skills Demonstrated
- Data Cleaning
- Data Transformation
- Data Modeling Basics
- DAX Calculations
- KPI Development
- Data Visualization
- Business Intelligence
- Interactive Dashboard Development
- Business Insights Generation

## 🚀 Project Outcome
Successfully developed an interactive Power BI dashboard that transforms raw retail sales data into meaningful business insights and helps understand sales performance across products, regions, months, and payment methods.

## 👩‍💻 Author
**Ashwini Jadhav**

Aspiring Data Analyst | Data Science Enthusiast

