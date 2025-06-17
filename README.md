# ☕ Coffee Orders Dashboard — Excel Data Analytics Project
## 📈 Overview
This project showcases a comprehensive sales analysis dashboard built entirely in Microsoft Excel, designed to provide actionable insights into coffee product performance, customer behavior, and sales trends. It demonstrates my proficiency in Excel functions such as XLOOKUP, INDEX+MATCH, IF, pivot tables, and dashboard design — skills essential for real-world data analysis.

### :dart: Key Highlights
✅ Customer & Product Lookup

Used XLOOKUP to retrieve customer details (Name, Country, Loyalty Status) based on Customer ID

Used INDEX + MATCH to dynamically pull product details (Coffee Type, Roast, Size, Price)


### ✅ Data Cleaning & Transformation

- Converted coffee type codes (e.g., "Ara") to full names using nested IF statements

- Transformed roast level abbreviations (e.g., "M") into readable values like "Medium"

- Formatted dates to dd/mmmm/yyyy for consistency

- Rounded product sizes to 1 decimal place and appended unit "kg"

- Applied USD formatting to all monetary values

- Checked and removed duplicates

- Structured the dataset into an Excel Table for easier referencing
### ✅ Sales Calculations

Added a calculated column:
= Unit_Price * Quantity_Sold
to compute the revenue per transaction

### ✅ Interactive Dashboard

- Created a pivot table-driven dashboard

- Used slicers for filters by Roast, Coffee Type, Country, and Customer Loyalty

- Included total KPIs, bar charts by coffee type and country, and time-based sales metrics

- Visualized insights across multiple sheets (Total_Sales, Country Sales, Coffee_Dashboard)

### 🧠 Skills Demonstrated
- 📈 Data Analysis & Visualization

- 🧹 Data Cleaning & Transformation

 - 🧩 Advanced Excel Functions (XLOOKUP, INDEX, MATCH, IF, TEXT, ROUND)

- 📊 Pivot Tables & Slicers

- 🧪 Problem Solving with Formula Logic

- 💼 Real-world Sales & Customer Data Modeling

### 📁 File Structure
- Sheet: Name	Description
- orders:	Cleaned order-level data with computed columns
- customers:	Customer information used for XLOOKUP
- products:	Product information used for INDEX+MATCH
- Total_Sales:	Aggregated coffee sales by year/month/type
- country_bar_char:	Bar chart of total sales by country
- Coffee_Dashboard:	Main interactive dashboard with filters and charts

🛠️ Sample Formulas
- XLOOKUP for Customer Name
* ` =XLOOKUP(C2,customers!$A$1:$A$1001,customers!$B$1:$B$1001,,FALSE) `
- INDEX + MATCH for Product Size
* `=INDEX(products!$A$1:$G$49,MATCH(orders!$D2,products!$A$1:$A$49,0),MATCH(orders!K$1,products!$A$1:$G$1,0))`
  
` =IF(I2="Rob","Robusta",IF(I2="Exc","Excelsa",IF(I2="Ara","Arabica",IF(I2="Lib","Librica",""))))`

- Date Formatting
` =TEXT([@Order_Date], "dd/mmmm/yyyy")`

- Size Formatting with Unit
` =ROUND([@Size], 1) & " kg" `

### 🔍 How to Use the Dashboard
- Open the file: Coffee Orders Dashboard(Beige).xlsx

- Explore each sheet: Check orders, Total_Sales, and the Coffee_Dashboard

- Use filters: Interact with slicers to view trends by country, roast, and loyalty

- Drill down: Use the pivot table to break down performance by product, time, and region

### 🚀 Why This Project Matters
This Excel dashboard simulates a real-world business case where a coffee company wants to:

1. Understand which products drive revenue

2. Track customer segments by region and loyalty

3. Make data-backed decisions from visual insights

👨‍💻 About Me
I'm a passionate data analyst focused on creating clean, insightful, and professional dashboards using tools like Excel, Power BI,Tableau and Python. This project reflects my ability to clean messy data, engineer insights, and present results clearly — all in Excel.

🤝 Let’s Connect
If you're a recruiter, company, or collaborator interested in data-driven work — I'm open to opportunities and discussions.

📧 Email: paakwesiprah20@gmail.com
🔗 LinkedIn: [LinkedIn](https://www.linkedin.com/in/prince-paakwesi-prah/)


