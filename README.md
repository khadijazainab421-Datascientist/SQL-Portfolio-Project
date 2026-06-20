# SQL Portfolio Project

## Project Overview
This project analyzes sales data using SQL and SQLite.

## Dataset
Sales dataset with order details, customers, regions, categories, sales, profit, and shipping information.

## Tools Used
- SQLite
- DB Browser for SQLite
- SQL
- GitHub

## SQL Analysis Performed
- Total Orders
- Total Sales
- Total Profit
- Top 5 Countries by Sales
- Top Categories by Sales

## Key Insights
- Total Orders: 28,989
- Total Sales: 4,444,935.5
- Total Profit: 799,859.47
- United States generated the highest sales.
- SQL queries were used to analyze sales performance by country and category.

## Sample Queries

```sql
SELECT COUNT(*) AS total_orders
FROM sales_data;

SELECT SUM(sales) AS total_sales
FROM sales_data;

SELECT country,
       SUM(sales) AS total_sales
FROM sales_data
GROUP BY country
ORDER BY total_sales DESC
LIMIT 5;

Author

Khadija Zainab
