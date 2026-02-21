# Sales-data-analysis-
SQL-based sales data analysis project exploring revenue trends, product performance, regional contribution, and salesperson rankings.

## Project Overview
This project analyzes a sales dataset using SQL to understand revenue trends, product performance, regional sales contribution, and salesperson performance.

The goal of this project is to practice writing SQL queries for business analysis and generate meaningful insights from transactional sales data.

---

## Dataset Information

Table Name: sales_data

Columns:
- order_id
- order_date
- region
- salesperson
- product
- category
- units_sold
- unit_price
- total_sales

The dataset contains 200+ sales records.

---

## Tools Used

- SQL (MySQL syntax)
- Excel (for dataset preparation)

---

## Key Analysis Performed

1. Total revenue and total units sold
2. Revenue by region
3. Revenue by product
4. Top performing salespersons
5. Monthly revenue trend
6. Best selling product by quantity
7. Region contribution percentage
8. Salesperson ranking using window functions
9. Month-over-month revenue growth

---

## Sample Query

```sql
SELECT region,
       SUM(total_sales) AS revenue
FROM sales_data
GROUP BY region
ORDER BY revenue DESC;
