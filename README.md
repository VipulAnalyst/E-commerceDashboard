SWYNEX: E-commerce Sales Analytics

Final data analytics project for Swynex, an e-commerce company. It takes a messy orders dataset through cleaning, exploratory analysis and an interactive Power BI dashboard, and ends with business insights and recommendations.

Dashboard

Problem Statement

How is Swynex's online store performing, and how far can its order data be trusted? The project looks at revenue and trends, top categories and cities, the effect of discounts and order status, and data-quality problems.

Dataset

Swynex e-commerce orders: 116 orders, 14 columns, 1 Jan to 25 Sep 2026 (one row per order). Columns: Order_ID, Customer_ID, Customer_Name, City, Order_Date, Product_ID, Product_Name, Category, Quantity, Unit_Price, Discount, Payment_Method, Order_Status, Total_Amount.

Process
Cleaning (data_cleaning.ipynb, pandas): dropped 2 rows with unparseable dates and flagged 3 anomaly rows: ORD0052 (Quantity -2), ORD0071 (Discount 110) and ORD0091 (Total_Amount 99,999).
EDA (EDA_data.ipynb): statistics, trends, category, city and payment breakdowns, anomaly checks.
Dashboard (Power BI): KPIs for revenue, delivered revenue, orders, average order value and cancellation rate, with charts by month, status, category, city and payment method. Built on dashboard_data.csv, where the 3 anomalies are repaired.
Key Insights
Electronics brings 46% of revenue; Bags have the highest average order value (Rs. 3,902).
Delhi NCR (Delhi, Gurugram, Noida) gives about half of revenue; August is the peak month (Rs. 59,517).
Only 54% of orders are delivered; cancelled and pending orders hold nearly half of order value.
Credit Card orders cancel most often (35.5%), UPI least (12%).
The data accepted impossible values, so input validation at order entry is recommended.
Repository Structure
Ecommerce-Dashboard/
├── README.md
├── report/      SWYNEX_Final_Data_Analytics_Report.pdf
├── data/        raw_messy_data.csv, cleaned_data.csv, dashboard_data.csv
├── notebooks/   data_cleaning.ipynb, EDA_data.ipynb
└── dashboard/   E_Commerce_Dashboard.pbix, dashboard.png
Tools

Python (pandas, matplotlib, seaborn), Jupyter in VS Code, Power BI, Excel, Git.

Links
Full report: report/SWYNEX_Final_Data_Analytics_Report.pdf
Task 1, cleaning: https://github.com/VipulAnalyst/ecommerce-data-cleaning
Task 2, EDA: https://github.com/VipulAnalyst/Ecommerce_eda
LinkedIn video: https://lnkd.in/p/gz_vMdu9

Author: Vipul Dubey | Data Analytics Internship, Swynex
