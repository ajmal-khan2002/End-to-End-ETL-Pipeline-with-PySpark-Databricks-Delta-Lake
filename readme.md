<H2>End-to-End ETL Pipeline with PySpark</H2>
A production-grade, scalable data engineering pipeline processing 46M+ records across ingestion, transformation, and Delta Lake layers — with 99.8% data validity and 12 business-focused analytical use cases.<br>

<H1>ETL Architecture</H1>

<img width="465" height="181" alt="Screenshot 2026-03-06 151712" src="https://github.com/user-attachments/assets/dd7277ce-8417-495e-80b4-d7e0d3965f5d" />

<h1>Business Cases</h1><br>
<h2>🔵 Level 1 — Core Analytics</h2><br>
1️⃣ Customer Lifetime Value (CLV)<br>
Business Question: Which customers generate the highest total revenue over their lifetime?
MetricDescriptionTotal OrdersCount of all orders per customerTotal RevenueSum of all revenue per customerAvg Order ValueAverage spend per orderFirst & Last OrderCustomer activity timeline
Tables Used: customers, orders<br>

2️⃣ Daily Revenue Trend<br>
Business Question: How does daily revenue change over time?<br>
MetricDescriptionRevenue Per DayTotal daily revenueOrder Count Per DayNumber of orders placed each dayFilterCancelled orders excluded<br>
Tables Used: orders<br>

3️⃣ Top Cities by Revenue<br>
Business Question: Which cities contribute the most revenue?<br>
MetricDescriptionTotal RevenueRevenue aggregated per cityUnique CustomersNumber of distinct customers per cityAvg Order ValueAverage order spend per city
Tables Used: orders, customers<br>

<h2>🟡 Level 2 — Intermediate Analytics</h2><br>
4️⃣ Repeat vs One-Time Customers<br>
Business Question: How many customers are repeat buyers vs one-time buyers?<br>
MetricDescriptionOne-Time BuyersCustomers with exactly 1 orderRepeat BuyersCustomers with more than 1 orderRevenue ContributionRevenue split by each group
Tables Used: customers, orders<br>

5️⃣ Order Fulfillment Performance<br>
Business Question: What percentage of orders are delivered vs cancelled?<br>
MetricDescriptionOrder Count by StatusCount grouped by order statusPercentage ShareStatus breakdown as % of totalDaily BreakdownStatus trends over time
Tables Used: orders<br>

6️⃣ Revenue by Payment Method<br>
Business Question: Which payment methods drive the most revenue?<br>
MetricDescriptionRevenue by MethodTotal revenue per payment typeFilterCancelled orders excluded
Tables Used: orders

<h2>🔴 Level 3 — Advanced Analytics</h2><br>
7️⃣ Product Category Performance<br>
Business Question: Which product categories generate the most revenue?<br>
MetricDescriptionRevenue by CategoryRevenue broken down by category & sub-categoryQuantity SoldTotal units sold per categoryTop 5 ProductsHighest-performing products per category
Tables Used: order_items, products<br>

<h2>⚙️ Key Features</h2><br>

✅ Scalable ETL pipelines using factory design patterns for modular, reusable code<br>
✅ 99.8% data validity through schema enforcement and data quality checks<br>
✅ Delta Lake integration with ACID transactions, upserts, and time travel<br>
✅ Processes 46M+ records end-to-end across all pipeline layers<br>
✅ 12 business-focused analytical use cases spanning 3 complexity levels<br>


🚀 Getting Started<br>
Prerequisites<br>

Python 3.8+<br>
Apache Spark 3.x<br>
Databricks Runtime (recommended)<br>
Delta Lake 2.x<br>

🤝 Contributing<br>
Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.<br>

Built with using PySpark, Databricks & Delta Lake<br>

Auther : Ajmal Khan<br>
