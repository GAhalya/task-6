📊**Sales Trend Analysis Using Aggregations**
📌 **Overview**
This project demonstrates how to perform sales trend analysis in SQL using aggregation functions and related clauses. The goal is to explore customer, product, and order data to derive meaningful insights such as monthly sales trends, product performance, and country-wise distribution of customers.

🎯 **Objectives**
- Extract useful time-based data for trend analysis.
- Aggregate and summarize sales-related information.
- Organize results for better readability and interpretation.

🛠️ **SQL Concepts Covered**
- EXTRACT() – Extract month from an order date to analyze sales seasonality.
- GROUP BY – Group data by categories (e.g., country) to analyze distribution.
- SUM() – Calculate total quantities sold.
- COUNT(DISTINCT) – Count unique items or customers.
- ORDER BY – Sort results based on a specific column (e.g., price).

📂 **Queries and Outputs**
## 1. Extract Month from Order Date
   **Query**: SELECT EXTRACT(MONTH FROM '2017-06-15');
✅ Helps in grouping and analyzing sales per month.

## 2.  Group Customers by Country
    **Query** :SELECT COUNT(customer_id), country
           FROM customers
           GROUP BY country;
✅ Shows how many customers belong to each country.

## 3. Calculate Total Quantity Sold
   **Query**: SELECT SUM(quantity)
          FROM orderdetails;
✅ Useful for understanding total product demand.

## 4. Count Unique Products
   **Query**: SELECT COUNT(*)
          FROM products;
✅ Determines the number of distinct products available.

## 5. Sort Products by Price
   **Query**: SELECT * FROM products
          ORDER BY price;
✅ Helps in price-based analysis and finding top/bottom priced items.

📈 **Insights You Can Derive**
- Monthly trends to identify peak sales seasons.
- Country-level customer distribution for targeted marketing.
- Top-selling product quantities to manage inventory.
- Price-based product ranking for pricing strategy decisions.
