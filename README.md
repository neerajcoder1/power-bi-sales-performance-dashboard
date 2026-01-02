# power-bi-sales-performance-dashboard
Sales Performance &amp; Delivery Insights Dashboard using Power BI
# 📊 Sales Performance & Delivery Insights Dashboard

## 📌 Project Overview
This Power BI dashboard analyzes sales performance across products, categories, and states.
It also highlights delivery efficiency and customer payment behavior to support business decision-making.

## 🛠 Tools Used
- Power BI
- DAX
- Microsoft Excel

## 📈 Key Metrics
- Total Sales
- Total Orders
- Average Delivery Days
- Sales by Category
- Sales by State
- Payment Method Usage %

## 📊 Dashboard Insights
- Identified top-selling products and categories
- Analyzed regional sales performance across Indian states
- Evaluated customer payment preferences
- Measured delivery efficiency using average delivery days

## 📂 Files in Repository
- `Sales_Dashboard.pbix` → Power BI dashboard file  
- `Sales_Data.xlsx` → Source dataset  
- `dashboard.png` → Dashboard preview image  

## 🧠 Key DAX Measures
```DAX
Total Sales = 
SUMX ( Sales_Data, Sales_Data[Quantity] * Sales_Data[Unit_Price] )

Net Sales =
[Total Sales] - [Total Discount]

Average Delivery Days =
AVERAGE ( Sales_Data[Delivery_Days] )
