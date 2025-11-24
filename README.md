
# 🛒 Superstore Sales Data Analysis
A complete data analysis project using **Python, Pandas, NumPy, Matplotlib, and Seaborn** to explore sales performance, profit trends, customer behavior, and shipping analysis.

---

## 📌 Project Overview
The Superstore dataset contains information about orders, customers, sales, region-wise performance, and shipping.  
This project focuses on **data cleaning, EDA (Exploratory Data Analysis), and generating actionable insights** that can help understand business performance.

---

## 🎯 Objectives of the Project
- Identify **top performing categories & sub-categories**
- Find **most profitable and least profitable regions**
- Analyze **sales vs profit relationship**
- Study **shipping delays**
- Understand **customer buying patterns**
- Detect performance trends across **segments and regions**

---

## 📊 Dataset Description
**Rows:** ~10k (approx)  
**Columns:** Customer info, Orders, Sales, Profit, Region, Category, Sub-Category, Ship Mode, Dates, etc.

Important Columns:
- Order Date  
- Ship Date  
- Order ID  
- Customer Name  
- Segment  
- City / State / Region  
- Category / Sub-Category  
- Sales  
- Profit  
- Quantity  
- Discount  
- Ship Mode  

---

## 🧼 Data Cleaning Steps
- Handled missing values  
- Converted `Order Date` & `Ship Date` to datetime  
- Created new column:  
  ```python
  df['Shipping Delay'] = (df['Ship Date'] - df['Order Date']).dt.days
