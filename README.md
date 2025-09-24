# Superstore Sales Dashboard (Power BI)

## 📌 Project Overview
This project presents a **Sales & Profit Dashboard** built in **Power BI** using the Superstore dataset.  
The dashboard highlights sales trends, profit analysis, customer insights, and regional performance.  
Final deliverables include a Power BI dashboard and a PDF report for business storytelling.

---

## 📊 Dataset
- **Source:** Sample Superstore dataset (`Superstore.csv`)  
- **Fields:**  
  - Dimensions: Order ID, Order Date, Customer, Segment, Region, State, Category, Sub-Category, Product Name  
  - Measures: Sales, Quantity, Discount, Profit  

---

## 🎯 Objectives
- Track **Sales & Profit trends** over time  
- Identify **top-performing categories and products**  
- Compare **regional & customer performance**  
- Analyze **discount impact on profit margins**  
- Provide **business recommendations**  

---

## 📖 Dashboard Pages
1. **Executive Summary** – KPIs & sales/profit trend  
2. **Category & Product Analysis** – Contribution & profitability  
3. **Geography Performance** – Sales by region/state  
4. **Customer & Segment Insights** – Top customers, segment analysis  
5. **Recommendations** – Key takeaways & actions  

---

## 🔢 Key DAX Measures
```DAX
Total Sales = SUM(Superstore[Sales])
Total Profit = SUM(Superstore[Profit])
Profit Margin = DIVIDE([Total Profit], [Total Sales], 0)
Order Count = DISTINCTCOUNT(Superstore[Order ID])
Avg Order Value = DIVIDE([Total Sales], [Order Count], 0)
