# Data-Analysis-Sales-Insights-Project-using-Python-and-Power-BI
**Project Overview**

The Sales Insights Dashboard is a data analysis and visualization project designed to provide deep insights into sales performance across products, markets, customers, and time. The goal of this project is to help businesses track revenue, profit, and customer behavior trends while identifying key drivers of growth and underperforming areas.

Using Python for preprocessing,and Power BI for visualization, this project delivers a comprehensive and interactive reporting system for data-driven decision-making.

**Objectives**

Build an automated dashboard to track sales KPIs.

Analyze revenue and profit trends over time.

Identify top customers, products, and markets contributing to sales.

Segment customers by type (e-commerce, brick & mortar) and analyze profitability by zones.

Provide geographical insights with a location-based revenue map.

**Tools & Technologies**

Python (Pandas, NumPy, Matplotlib) – Data cleaning, preprocessing, and exploration

Power BI – Dashboard creation, KPI tracking, interactive reports

DAX (Data Analysis Expressions) – Measures for revenue, profit, trends, and segmentation

Power Query (M Language) – ETL transformations

Data Modeling – Star Schema (Fact & Dimension tables)

**Key Features of the Dashboard**

KPIs: Total Products Sold, Total Revenue, Total Profit

Trend Analysis: Revenue vs Profit across months/years

Market Insights: Revenue and Profit by Market & Zone

Customer Insights: Revenue by Customer Type and Top 5 Customers

Product Analysis: Top Products by Sales

**Relationships**
![image alt](https://github.com/VaishnaviGhorpade99/Data-Analysis-Sales-Insights-Project-using-Python-and-Power-BI/blob/main/Relationships..png)

**Data Model**

The dashboard follows a Star Schema design for efficient analytics:

Fact Table: Sales (Quantity, Revenue, Profit, Date, CustomerID, ProductID, MarketID)

Dimension Tables: Customers, Products, Markets, Date

**DAX Measures** (Examples)
Total Revenue = SUM(FactSales[Revenue])
Total Profit = SUM(FactSales[Profit])
Total Products Sold = SUM(FactSales[Quantity])

Revenue % by Zone =
DIVIDE(
    SUM(FactSales[Revenue]),
    CALCULATE(SUM(FactSales[Revenue]), ALL(DimMarket))
)

 **Business Impact**

Enabled stakeholders to track sales performance in real-time.

Identified top customers, products, and high-revenue markets.

Improved strategic decision-making with insights on revenue drivers and low-performing zones.

Provided an automated, interactive reporting solution reducing manual report creation time.

**Dashboard Preview**

📂 Repository Structure
├── data/                # Raw and processed datasets  
├── scripts/             # Python preprocessing scripts  
├── queries/             # SQL queries for data extraction  
├── dashboard/           # Power BI .pbix file  
└── README.md            # Project documentation  

**Future Enhancements**

Add predictive analytics for sales forecasting.

Integrate with Power Automate for scheduled refreshes.

Extend dashboard to include customer churn analysis.

**Dashboard Preview**

![image alt](https://github.com/VaishnaviGhorpade99/Data-Analysis-Sales-Insights-Project-using-Python-and-Power-BI/blob/main/Dashboard.png)
