# Task 6: Sales Trend Analysis Using Aggregations

## Objective
Analyze monthly revenue and order volume from online sales.

## Dataset
Contains `order_id`, `order_date`, `amount`, `product_id` for 2000 orders.

## Queries Performed
- Monthly Revenue & Volume
- Top 3 Revenue Months
- Null Handling
- Count(*) vs Count(DISTINCT)

## Tools Used
- MySQL
- SQL Queries

## Sample Query
```sql
SELECT YEAR(order_date), MONTH(order_date), SUM(amount) FROM online_sales GROUP BY 1, 2;
