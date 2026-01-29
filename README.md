# Superstore SQL Business Insights (Google BigQuery)

## Project Overview
This project analyzes retail sales data using SQL to uncover revenue drivers, profit trends, and operational risks.  
The analysis was performed in **Google BigQuery** using the Superstore dataset to demonstrate practical, business-focused SQL skills.

The goal is to answer real business questions that stakeholders care about — not just write queries.

---

## Business Questions Answered
- What are total sales, profit, and order volume?
- Which product categories and sub-categories are most profitable?
- Which products are losing money?
- How does profit vary by region?
- What does the monthly sales trend look like over time?
- How do discounts impact profitability?

---

## Tools Used
- Google BigQuery (SQL)
- Public Superstore dataset
- GitHub for version control and documentation

---

## Key SQL Queries Included
All queries are stored in `queries.sql`, including:
- Total sales, profit, and orders
- Sales by category
- Profit by region
- Monthly sales trends
- Most profitable sub-categories
- Loss-making sub-categories
- Profit margin by category

---

## Key Findings
- **Technology** generates the highest overall profit margin, while Furniture lags significantly.
- **Several sub-categories consistently lose money**, indicating pricing or cost issues.
- **Sales peak seasonally toward year-end**, showing strong Q4 demand patterns.
- Higher discount bands correlate with **lower overall profitability**.

---

## Recommendations
- Re-evaluate discounting strategies for low-margin and loss-making products.
- Prioritize inventory and marketing efforts ahead of Q4 seasonal demand.
- Review pricing, shipping costs, or supplier agreements for underperforming sub-categories.

---

## Screenshots

### Total Sales, Profit, and Orders
![Totals](screenshots/totals.png)

### Profit Margin by Category
![Profit Margin](screenshots/profit_margin.png)

### Monthly Sales Trend
![Monthly Sales](screenshots/monthly_sales.png)

---

## How to Run
1. Upload the Superstore dataset to Google BigQuery.
2. Create a table named `orders`.
3. Run the queries in `queries.sql`.
4. Review results and insights.

---

## Author
Hayward Collins  
Junior Data Analyst | SQL | Business Insights
