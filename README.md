# 📊 Simple Sales Dashboard (Power BI)

This project demonstrates how to create a **basic interactive sales dashboard** using **Power BI** and the **Superstore Sales dataset**.  
The dashboard highlights **sales performance by product category, region, and month** with interactive filtering options. 🚀  

---

## 📁 Dataset
We used the **Superstore Sales dataset** (commonly available in Tableau/Power BI sample data).  
Columns include:  
- 📅 `Order Date`  
- 🌍 `Region`  
- 🏷️ `Category`  
- 💰 `Sales`  
- 📈 `Profit`  

---

## 🛠 Tools Used
- **Power BI Desktop** 🟨  
- **Python + Pandas** 🐍 for data cleaning ( Optional)

---

## 📝 Steps Followed
1. **Imported the dataset** (`Superstore_Sales.csv`) into Power BI.  
2. **Converted** `Order Date` column into **Month–Year format** using DAX:  
   ```DAX
   MonthYear = FORMAT('Orders'[Order Date], "MMM yyyy")
   MonthYearSort = YEAR('Orders'[Order Date]) * 100 + MONTH('Orders'[Order Date])
Created visuals:

📈 Line Chart: Sales over Months

📊 Bar Chart: Sales by Region

🍩 Donut Chart: Sales by Category

3.**Added a slicer for Region to enable filtering.**

---



💡 Insights
From the dashboard, we can observe:

🌍 West Region recorded the highest sales overall.

📅 Sales peaked in 2017, showing strong year-end demand.

🏷️ Office Supplies category contributed the largest share of revenue (~60.3 %).


