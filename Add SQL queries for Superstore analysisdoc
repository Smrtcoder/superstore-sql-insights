-- Superstore SQL Business Insights
-- Author: Hayward Collins III

-- Query 1: Total Sales, Profit, Orders
SELECT
  ROUND(SUM(sales), 2) AS total_sales,
  ROUND(SUM(profit), 2) AS total_profit,
  COUNT(DISTINCT `Order ID`) AS total_orders
FROM superstore.orders;

-- Query 2: Sales by Category
SELECT
  category,
  ROUND(SUM(sales), 2) AS total_sales
FROM superstore.orders
GROUP BY category
ORDER BY total_sales DESC;

-- Query 3: Profit by Region
SELECT
  region,
  ROUND(SUM(profit), 2) AS total_profit
FROM superstore.orders
GROUP BY region
ORDER BY total_profit DESC;

-- Query 4: Monthly Sales Trend
SELECT
  DATE_TRUNC(`Order Date`, MONTH) AS month,
  ROUND(SUM(sales), 2) AS total_sales
FROM superstore.orders
GROUP BY month
ORDER BY month;

-- Query 5: Top Profitable Sub-Categories
SELECT
  `Sub-Category` AS sub_category,
  ROUND(SUM(profit), 2) AS total_profit
FROM superstore.orders
GROUP BY sub_category
ORDER BY total_profit DESC
LIMIT 10;

-- Query 6: Loss-Making Sub-Categories
SELECT
  `Sub-Category` AS sub_category,
  ROUND(SUM(profit), 2) AS total_profit
FROM superstore.orders
GROUP BY sub_category
HAVING SUM(profit) < 0
ORDER BY total_profit ASC;

-- Query 7: Profit Margin by Category
SELECT
  category,
  ROUND(SUM(profit) / NULLIF(SUM(sales), 0) * 100, 2) AS profit_margin_pct
FROM superstore.orders
GROUP BY category
ORDER BY profit_margin_pct DESC;
