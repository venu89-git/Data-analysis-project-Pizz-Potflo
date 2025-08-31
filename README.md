# Data-Analysis-project-Pizz-Potflo
## 🎯 Project Objective (for your Pizza Sales Dashboard)

The main objective of this project is to analyze pizza sales data to gain valuable business insights and improve decision-making.

.Specifically, the project aims to:

- 1.Understand Sales Performance

Track revenue, total orders, and average order value.

Identify the most profitable pizza categories and sizes.

- 2.Identify Customer Behavior & Trends

Find the busiest sales days and times (daily & hourly trends).

Discover ordering patterns (e.g., lunch vs. dinner peak hours).

Product Insights

Highlight the best-selling pizzas that drive sales.
Identify the worst-performing pizzas for possible improvement or removal.


- 3.Business Strategy Support

Provide actionable insights for marketing (promotions at peak times).

Optimize inventory based on popular sizes & categories.

Guide menu decisions (expand on popular pizzas, reconsider low-performing ones).


## Dataset Used
- <a href="https://github.com/venu89-git/Data-analysis-project-Pizz-Potflo/blob/main/project_pizz_potflo.xlsx"

## 📊 Key Performance Indicators (KPIs)

- 1.Revenue Metrics

Total Revenue 💵

Average Order Value (AOV) 💲

- 2.Order Metrics

Total Orders 📦

Total Pizzas Sold 🍕

Average Pizzas per Order

- 3.Trend Metrics

Daily Order Trend (orders by day of week)

Hourly Order Trend (orders by hour)

- 4.Category & Size Metrics

% Sales by Pizza Category

% Sales by Pizza Size

Total Pizzas Sold by Category

- 5.Product Performance Metrics

Top 5 Best-Selling Pizzas

Bottom 5 Worst-Selling Pizzas


## 📝 Step-by-Step Project Process (Updated)
- Step 1: Collect & Understand Data

Original pizza sales data is stored in SQL Server database.

Dataset includes: order_id, order_date, pizza_name, category, size, quantity, price.

✅ Protection: Keep a backup copy of the raw database (full dump or .bak file).

- Step 2: Connect SQL Server to Excel

Open Excel → Data → Get Data → From Database → From SQL Server.

Enter Server name and Database name.

Use either Direct Query (live connection) or Import (static snapshot).

Load the required tables or views (e.g., orders, pizzas, sales).

✅ Protection:

Create a read-only user in SQL Server for reporting (prevents accidental changes to live data).

Store connection strings securely (avoid sharing passwords in GitHub).

- Step 3: Data Cleaning

In Excel Power Query Editor, clean the imported data:

Remove duplicates, nulls.

Standardize category/size.

Add calculated columns (e.g., Revenue = Quantity × Price).

✅ Protection: Save queries as .pq steps (so cleaning is reproducible).

- Step 4: Data Analysis

Build pivot tables and charts in Excel.

Aggregate data by day, hour, category, size.

Calculate metrics: Total Revenue, Orders, Pizzas Sold, AOV.

✅ Protection: Keep a log of transformations inside SQL (views or stored procedures).

- Step 5: Dashboard Creation

Create KPIs:

Total Revenue

Avg Order Value

Total Orders

Avg Pizzas per Order

Add charts for:

Sales trend (daily & hourly)

Category & size distribution

Top 5 / Bottom 5 pizzas

✅ Protection: Save dashboard separately (pizza_dashboard.xlsx). Keep a backup copy.

- Step 6: Insights & Documentation

Document findings (e.g., busiest hours, best sellers).

Write insights in a README.md for GitHub.

S- tep 7: Version Control & Sharing

Upload project to GitHub.

Do not upload raw SQL database (security risk).

Instead, upload:

dashboard.xlsx (with SQL connection details hidden).

docs/ folder (with instructions & screenshots).

requirements.md (Excel version, SQL version).

Share sample dataset instead of full data.

✅ Protection: Keep repository private if database is confidential.


## Dashbord Interaction <a href="https://github.com/venu89-git/Data-analysis-project-Pizz-Potflo/blob/main/Screenshot%202025-08-30%20200556.png"

  

# 📊 About the SQL Queries

In this project, SQL Server was used to extract and analyze pizza sales data.
The queries were designed to answer key business questions and generate the metrics used in the dashboard.

- 1. KPI Queries

These queries calculate the core business metrics:

Total Revenue – the sum of all sales.

Average Order Value – the average revenue per order.

Total Pizzas Sold – the total quantity of pizzas sold.

Total Orders – the number of unique customer orders.

Average Pizzas per Order – how many pizzas are included in a typical order.

- 2. Trend Analysis Queries

These queries show when customers order the most:

Daily Trend – orders broken down by day of the week (to see which days are busiest).

Hourly Trend – orders broken down by hour (to find peak lunch and dinner times).

- 3. Sales by Category & Size

These queries analyze customer preferences:

% of Sales by Category – revenue share for Classic, Chicken, Veggie, and Supreme pizzas.

% of Sales by Size – revenue share for Small, Medium, Large, and X-Large pizzas.

Total Pizzas Sold by Category – which categories sell the most in a given month.

- 4. Product Performance

These queries highlight best and worst performing pizzas:

Top 5 Best Sellers – most popular pizzas by quantity sold.

Bottom 5 Worst Sellers – least popular pizzas by quantity sold.

- 5. Filters & Customization

The queries can be filtered by Month, Quarter, or Week to focus on a specific time period.
For example:

January sales only.

First quarter sales.

Weekly breakdowns.

✅ In summary:
The SQL queries act as the backbone of the dashboard, feeding Excel or Power BI with accurate data for KPIs, trends, and insights.

## 📊 SQL Queries Document 

All the key KPIs, trends, and insights in this dashboard were generated using SQL Server queries.
👉 You can find the full list of queries here: <a href="https://github.com/venu89-git/Data-analysis-project-Pizz-Potflo/blob/main/PIZZA%20SALES%20SQL%20QUERIES.docx.pdf"
