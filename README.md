Financial Performance Dashboard

🎯 Project Objective

The objective of this project is to analyze Western Countries Financial Data to uncover insights into sales, profit, and product performance across different countries and segments.
The goal was to apply Excel, SQL, and Power BI skills to clean, analyze, and visualize the dataset, and finally create an interactive dashboard that highlights key business metrics for data-driven decisions.


---

📂 Dataset Used

 


---

❓ Business Questions (KPIs)

What are the total sales, profit, and units sold?

Which products drive the most sales and profit?

What is the segment-wise and product-wise performance?

What are the yearly and quarterly sales/profit trends?

Which countries contribute the most to revenue and profit?

Which are the Top 2 countries and Bottom 3 products?

What are the product-wise discounts?

What is the Year-over-Year (YoY) growth in units sold and sales?


📊 Dashboard Interaction: 
<img width="1226" height="697" alt="Screenshot 2025-08-31 152922" src="https://github.com/user-attachments/assets/2830096d-99fb-42cc-99f7-87916515f30a" />
<img width="1242" height="689" alt="Screenshot 2025-08-31 152851" src="https://github.com/user-attachments/assets/5570b481-9740-4723-98b2-adf4f942ad97" />
<img width="1218" height="689" alt="Screenshot 2025-08-31 153051" src="https://github.com/user-attachments/assets/cbfcf5d4-dde9-40ae-89b0-c3de23c7982e" />

---

⚙️ Process

1. Excel → Explored, cleaned dataset, handled missing values, removed duplicates.


2. Statistical Analysis → Summarized key metrics, identified outliers, calculated averages.


3. SQL → Imported dataset, created database & tables, validated data with queries, calculated KPIs.


4. Power BI →

Imported SQL data

Cleaned & transformed using Power Query

Created DAX measures (Total Sales, Total Profit, YoY Sales %, Total Units Sold)

Designed interactive visuals (sales, profit, units by product, country, segment)



5. Dashboard Design → Structured layout with slicers, KPIs, and interactive visuals for storytelling.




---

📊 Dashboard Highlights

Total Sales: 118.73M

Total Profit: 16.89M

Total Units Sold: 1.13M


📈 Key Insights:

Sales grew significantly from 2013 → 2014

USA & Canada were top-performing countries

Paseo was the best-selling product, while Amarilla & VTT underperformed

Small Business segment was most profitable, while Midmarket & Channel Partners reported losses

Discounts varied widely by product and segment, impacting profitability



---

📷 Dashboard Preview

<img width="1226" height="697" alt="Screenshot 2025-08-31 152922" src="https://github.com/user-attachments/assets/136abe87-9e6d-4ffe-bfd7-8c429ae0d411" />
<img width="1242" height="689" alt="Screenshot 2025-08-31 152851" src="https://github.com/user-attachments/assets/94d8fd07-aa79-45fb-aa42-c9e3c11d5861" />
<img width="1218" height="689" alt="Screenshot 2025-08-31 153051" src="https://github.com/user-attachments/assets/35d52ea3-8e24-4c0b-9cb0-b2f132732d44" />


---

📐 Sample Queries & DAX

SQL – Yearly Sales & Profit

SELECT Year, SUM(Sales) AS TotalSales, SUM(Profit) AS TotalProfit
FROM western
GROUP BY Year
ORDER BY Year;

DAX – Total Sales

Total Sales = SUM(financials[Sales])

DAX – YoY Sales %

YoY Sales % =
DIVIDE(
    [Total Sales] - CALCULATE([Total Sales], SAMEPERIODLASTYEAR('DateTable'[Date])),
    CALCULATE([Total Sales], SAMEPERIODLASTYEAR('DateTable'[Date]))
)


---

📈 Learnings

Hands-on practice with data cleaning & ETL in Excel

Building SQL queries for KPIs & validation

Creating DAX measures and applying time intelligence functions

Designing interactive dashboards in Power BI

Improving data storytelling through visualization



---

🤝 Connect With Me

💼 LinkedIn

📂 GitHub



---

🔥 This project was an end-to-end journey from raw data to actionable insights and interactive dashboards.


---

