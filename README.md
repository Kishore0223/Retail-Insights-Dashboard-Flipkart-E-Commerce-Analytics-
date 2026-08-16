# Retail-Insights-Dashboard-Flipkart-E-Commerce-Analytics-
An interactive Power BI dashboard analyzing seller, sales, and delivery performance across a Flipkart-style e-commerce dataset. The report is organized into a landing/navigation page and three analytical pages, letting stakeholders drill from top-line KPIs down into category, seller, and delivery-level detail.
Data Model
Fact table: flipkart_cleaned — cleaned e-commerce transaction data (~80K rows) covering products, categories, brands, sellers, seller cities, order values, units sold, stock, ratings, discounts, and delivery timelines.
Dimension table: Date Table — supports time intelligence (monthly/yearly trend analysis).
Single-fact-table star-schema style model with one relationship to the date dimension.
Pages
1. Home

Navigation landing page with three action buttons routing to each analysis page:

Executive summary — "Top-line KPIs at a glance"

Sales and revenue — "Trends, category and channel performance"

Seller and delivery — "Fulfilment, delays and seller ratings"

2. Executive Overview

KPI summary and top-line trend view.

KPI cards: Total Revenue, Total Units Sold, Average Rating, Return Rate %, Average Discount %

Line chart: Total Revenue trend by month

Bar chart: Total Revenue by category

Donut chart: Units sold share by seller

Slicers: Year, Category, Seller City

3. Sales & Revenue Performance

Deeper revenue breakdown.

Pivot table: Category × Brand with units sold, total revenue, and average rating

Map: Revenue by seller city

Clustered bar chart: Top 10 products by revenue

4. Seller & Delivery Performance

Fulfilment and seller quality analysis.

Scatter chart: Seller rating vs. average delivery days (bubble size = units sold)

Bar chart: Average delivery days by city

Table: Seller-level view of total revenue, return rate %, average rating, and stock available

KPI card: Low Stock Products

Key DAX Measures

Total Revenue

Total Units Sold

Average Rating

Return Rate %

Average Discount %

Average Delivery Days

Top Category by Revenue

Low Stock Products

Tools Used

Power BI Desktop — data modeling, DAX, report design

Power Query — data cleaning (flipkart_cleaned table)

DAX — KPI and time-intelligence measures
Dataset

Flipkart-style e-commerce dataset (~80,000 rows) covering product, seller, order, and delivery attributes.
