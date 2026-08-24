# Superstore Sales Dashboard (Power BI)

## Project Overview

The **Superstore Sales Dashboard** is an interactive business intelligence dashboard developed using **Microsoft Power BI Desktop**. It provides a comprehensive overview of sales performance, profitability, orders, and quantity through dynamic KPI cards, interactive slicers, and insightful visualizations.

The dashboard enables business users and decision-makers to monitor key performance indicators (KPIs), analyze sales trends across categories and states, and make informed decisions based on real-time filtering.

---

# Objectives

* Develop an interactive sales dashboard using Power BI.
* Monitor business performance using Executive KPI cards.
* Analyze sales and profit by category and state.
* Identify the top-performing sub-categories.
* Provide interactive filtering for quick business insights.

---

# Tools & Technologies

* **Microsoft Power BI Desktop**
* **Power Query**
* **DAX (Data Analysis Expressions)**
* **CSV Dataset**
* **Data Modeling**

---

# Dataset Information

The dashboard is built using a Superstore Sales dataset containing information such as:

* Order ID
* Order Date
* Customer Name
* Category
* Sub-Category
* City
* State
* Payment Mode
* Quantity
* Amount (Sales)
* Profit

---

# Dashboard Features

## Executive KPI Cards

The dashboard displays the following KPIs:

* Total Sales
* Total Profit
* Total Orders
* Total Quantity
* Profit Margin (%)

These KPI cards dynamically update based on the selected slicers.

---

## Category Performance Analysis

Provides detailed analysis of:

* Sales by Category
* Profit by Category
* Top 10 Sub-Categories by Sales

This section helps identify the highest-performing product categories.

---

## Regional (State) Profitability Analysis

Displays:

* Sales by State
* Profit by State
* State Profit Margin

This visualization helps compare business performance across different states.

---

## Interactive Slicers

The dashboard includes slicers for:

* City
* Year
* State
* Category
* Payment Mode

Users can filter the entire dashboard instantly using these slicers.

---

# DAX Measures Used

```DAX
Total Sales =
SUM('Sales Dataset'[Amount])

Total Profit =
SUM('Sales Dataset'[Profit])

Total Orders =
DISTINCTCOUNT('Sales Dataset'[Order ID])

Total Quantity =
SUM('Sales Dataset'[Quantity])

Average Sales =
AVERAGE('Sales Dataset'[Amount])

Profit Margin % =
DIVIDE([Total Profit],[Total Sales],0)

State Profit Margin =
DIVIDE([Total Profit],[Total Sales],0)
```

---

# Dashboard Components

* Dashboard Title
* Executive KPI Cards
* Category Analysis Charts
* State-wise Sales Analysis
* State-wise Profit Analysis
* State Profit Margin Analysis
* Interactive Slicers

---

# Key Insights

* Displays total business sales and profit.
* Identifies the best-performing product categories.
* Highlights the highest-selling sub-categories.
* Compares sales and profit across different states.
* Calculates overall profit margin.
* Enables dynamic business analysis using slicers.

---

# Benefits

* Easy to understand and interactive.
* Supports faster business decision-making.
* Provides a real-time overview of sales performance.
* Improves reporting efficiency.
* Professional executive dashboard design.

---

# Future Enhancements

* Monthly and yearly sales trend analysis.
* Customer segmentation dashboard.
* Product performance forecasting.
* Sales target vs actual comparison.
* Inventory and stock monitoring.
* Integration with SQL Server or cloud databases.
* Automated dashboard refresh using Power BI Service.

---

# Conclusion

The **Superstore Sales Dashboard** demonstrates the effective use of **Power BI** for transforming raw sales data into meaningful business insights. Through interactive KPI cards, dynamic filtering, and visually appealing charts, the dashboard enables users to analyze sales, profitability, and regional performance efficiently. It serves as a practical business intelligence solution for monitoring organizational performance and supporting data-driven decision-making.

---

**Dashboard Summary**

* **Project Title:** Superstore Sales Dashboard
* **Tool Used:** Microsoft Power BI Desktop
* **Data Source:** CSV Dataset
* **Visualization Type:** Interactive Dashboard
* **Dashboard Includes:** KPI Cards, Bar Charts, Column Charts, Slicers, Profitability Analysis
