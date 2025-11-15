FUTURE_DS_01 — Business Sales Dashboard (E-Commerce Data Analytics)

📘 Project Overview
This project is part of my **Data Science & Analytics Internship** at **Future Interns**.  
The goal is to analyze e-commerce sales data and build an **interactive Power BI dashboard** that helps business leaders identify:
- Best-selling products  
- High-revenue categories  
- Monthly and regional sales trends  
- Overall profit performance  

The dashboard transforms raw transactional data into actionable insights to support data-driven decision-making.

---

🧠 Business Objective
E-commerce businesses handle thousands of transactions daily, making it essential to monitor sales patterns effectively.  
This dashboard provides:
1. **Real-time tracking** of key metrics (Sales, Orders, Profit, AOV).  
2. **Trend analysis** to highlight growth and seasonal demand.  
3. **Category and product-level insights** for business optimization.  

---

🧰 Tools & Technologies
| Category | Tools Used |
|-----------|-------------|
| Data Cleaning | Microsoft Excel |
| Data Visualization | Microsoft Power BI |
| Calculations | DAX (Data Analysis Expressions) |
| Dataset | Superstore (E-Commerce Dataset) |
| Version Control | GitHub |

---

🔍 Workflow

1️⃣ Data Preparation
- Imported dataset `superstore.xlsx` into Power BI.
- Cleaned missing or duplicate records.
- Standardized column names and data types (especially *Date*, *Sales*, *Profit*).
- Created a calendar table for time intelligence.

2️⃣ Data Modeling
- Built relationships between tables: *Orders*, *Products*, and *Customers*.
- Ensured a one-to-many structure for accurate aggregations.

3️⃣ DAX Calculations
Key measures created:
```DAX
Total Sales = SUM(Orders[Sales])
Total Orders = COUNTROWS(Orders)
Average Order Value = [Total Sales] / [Total Orders]
Profit Margin = DIVIDE(SUM(Orders[Profit]), [Total Sales])
Sales Growth % = 
   DIVIDE([Total Sales] - CALCULATE([Total Sales], DATEADD('Date'[Date], -1, MONTH)),
          CALCULATE([Total Sales], DATEADD('Date'[Date], -1, MONTH)))
```

4️⃣ Dashboard Design
Page 1 – Overview
KPIs: Total Sales, Profit, Orders, Average Order Value
Slicers: Year, Region, Category

Page 2 – Sales Analysis
Line Chart – Monthly Sales Trend
Bar Chart – Top 10 Products by Sales
Pie Chart – Sales by Category
Map – Regional Sales Distribution

Page 3 – Insights
Highlight cards summarizing key findings.
Narrative section explaining business takeaways.

📈 Key Insights
December shows the highest monthly revenue — likely due to seasonal demand.
Technology category contributes the largest profit margin.
Office Supplies have lower sales volume but steady performance across regions.
Top 5 products generate over 25% of total revenue — a potential focus for promotions.


📄 Summary Report Highlights
The Task1_Summary.pdf file in this repository includes:
Project background and objectives
Visual snapshots from Power BI
Key performance metrics and data-driven insights
Recommendations for sales and category optimization

🧩 Skills Demonstrated
Data Cleaning and Transformation
DAX Calculations for Business KPIs
Interactive Dashboard Design
Data Storytelling and Visualization
GitHub Documentation for Analytics Projects

👨‍💻 Author
Kumaravel B.
Data Science & Analytics Intern @ Future Interns
📧 kumaravelb9342@gmail.com
🔗 www.linkedin.com/in/kumaravel-b-7699ab2b0
🗓️ Internship Duration: November 2025 – December 2025
