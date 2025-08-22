# 📊 Sales-Dashboard-using-Excel  

### 📌 Project Overview  
This project analyzes **Softvision Communication’s 2024 Sales Performance** using Excel to build a dynamic and interactive sales dashboard.  
The dashboard provides a clear overview of **monthly revenue, top-performing products, customer segments, and regional performance**, allowing stakeholders to make **data-driven decisions**.  

---

### 🎯 Project Objectives / Problem Statement  
- Difficulty in **tracking and consolidating sales data** from different sources.  
- Lack of a **centralized dashboard** for management to quickly view performance metrics.  
- Limited ability to **identify trends and patterns** in sales growth.  
- Need for **better visualization** of KPIs (Revenue, Profit, Units Sold, Customer Segments).  

---

### 🔄 Process  
1. **Data Collection & Cleaning**  
   - Collected sales data (Excel format).  
   - Removed duplicates, handled missing values, standardized dates & formats.  

2. **Data Transformation**  
   - Applied **Power Query** to automate data cleaning and transformation.  
   - Merged multiple sheets/files into a consolidated dataset.  

3. **Dashboard Development**  
   - Built Pivot Tables & Charts in Excel.  
   - Applied slicers for interactive filtering (by Product, Region, Customer Type, etc.).  
   - Created KPIs (Total Revenue, Average Profit Margin, Growth Rate).  

---

### 🛠️ Tools  
- **Excel:** Data cleaning, pivot analysis, and dashboard design.  
- **SQL:** Querying structured datasets for deeper insights.  
- **Power BI:** For advanced visualization (future extension).  

---

### 📊 Key Insights  
- **Revenue Growth:** Sales revenue grew by **28.2%** in 2024 compared to 2023.  
- **Top Performer:** Digital Courses generated the highest revenue contribution (**16% of total sales**).  
- **Regional Insights:** Awka Sales Area outperformed other regions by **67.3%**.  
- **Customer Segment:** Corporate clients drove **41.8% of revenue**, highlighting B2B strength.  

---

### ⚡ Challenges and Solutions  
- **Challenge:** Raw sales data was inconsistent and scattered across files.  
  - ✅ **Solution:** Used **Power Query** to automate cleaning and merging.  
- **Challenge:** Manual reporting was time-consuming.  
  - ✅ **Solution:** Designed a **dynamic dashboard** that updates automatically.  
- **Challenge:** Lack of visibility on profit trends.  
  - ✅ **Solution:** Added KPIs and trend charts to highlight profitability.  

---

### 🔮 Future Work  
- Automate data pipeline using **SQL + Python** for scalability.  
- Expand dashboard to **Power BI** for richer visualization.  
- Integrate **forecasting models** to predict sales trends for 2025.  
- Develop a **customer segmentation model** for targeted marketing.  

---

### 🧩 Sample SQL Query  
```sql
SELECT 
    product_name, 
    SUM(revenue) AS total_revenue, 
    SUM(units_sold) AS total_units
FROM sales_data
JOIN customers ON sales_data.customer_id = customers.customer_id
GROUP BY product_name
ORDER BY total_revenue DESC;
