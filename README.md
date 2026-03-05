End-to-End ETL Pipeline with PySpark, Databricks & Delta Lake

A production-grade, scalable data engineering pipeline processing 46M+ records across ingestion, transformation, and Delta Lake layers — with 99.8% data validity and 12 business-focused analytical use cases.


📊 Business Use Cases
🔵 Level 1 — Core Analytics
1️⃣ Customer Lifetime Value (CLV)
Business Question: Which customers generate the highest total revenue over their lifetime?
MetricDescriptionTotal OrdersCount of all orders per customerTotal RevenueSum of all revenue per customerAvg Order ValueAverage spend per orderFirst & Last OrderCustomer activity timeline
Tables Used: customers, orders

2️⃣ Daily Revenue Trend
Business Question: How does daily revenue change over time?
MetricDescriptionRevenue Per DayTotal daily revenueOrder Count Per DayNumber of orders placed each dayFilterCancelled orders excluded
Tables Used: orders

3️⃣ Top Cities by Revenue
Business Question: Which cities contribute the most revenue?
MetricDescriptionTotal RevenueRevenue aggregated per cityUnique CustomersNumber of distinct customers per cityAvg Order ValueAverage order spend per city
Tables Used: orders, customers

🟡 Level 2 — Intermediate Analytics
4️⃣ Repeat vs One-Time Customers
Business Question: How many customers are repeat buyers vs one-time buyers?
MetricDescriptionOne-Time BuyersCustomers with exactly 1 orderRepeat BuyersCustomers with more than 1 orderRevenue ContributionRevenue split by each group
Tables Used: customers, orders

5️⃣ Order Fulfillment Performance
Business Question: What percentage of orders are delivered vs cancelled?
MetricDescriptionOrder Count by StatusCount grouped by order statusPercentage ShareStatus breakdown as % of totalDaily BreakdownStatus trends over time
Tables Used: orders

6️⃣ Revenue by Payment Method
Business Question: Which payment methods drive the most revenue?
MetricDescriptionRevenue by MethodTotal revenue per payment typeFilterCancelled orders excluded
Tables Used: orders

🔴 Level 3 — Advanced Analytics
7️⃣ Product Category Performance
Business Question: Which product categories generate the most revenue?
MetricDescriptionRevenue by CategoryRevenue broken down by category & sub-categoryQuantity SoldTotal units sold per categoryTop 5 ProductsHighest-performing products per category
Tables Used: order_items, products

⚙️ Key Features

✅ Scalable ETL pipelines using factory design patterns for modular, reusable code
✅ 99.8% data validity through schema enforcement and data quality checks
✅ Delta Lake integration with ACID transactions, upserts, and time travel
✅ Processes 46M+ records end-to-end across all pipeline layers
✅ 12 business-focused analytical use cases spanning 3 complexity levels


🚀 Getting Started
Prerequisites

Python 3.8+
Apache Spark 3.x
Databricks Runtime (recommended)
Delta Lake 2.x

🤝 Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

Built with using PySpark, Databricks & Delta Lake

Auther : Ajmal Khan