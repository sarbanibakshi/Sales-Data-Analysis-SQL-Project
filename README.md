# Sales-Data-Analysis-SQL-Project
This project follows a star schema approach with dimension tables for customers and products, and a fact table for sales transactions.

The repository includes:

* Table creation scripts
* Exploratory queries
* Business-focused analytical queries
* Key performance metrics and insights

## Dimension Table: gold.dim_customers

* Stores customer demographic and profile information.
* Customer identity and personal details
* Country, gender, marital status
* Birthdate and account creation date

## Dimension Table: gold.dim_products

* Contains product-level information.
* Product names and identifiers
* Category and subcategory hierarchy
* Product cost and product line details
* Effective start date

## Fact Table: gold.fact_sales

* Captures transactional sales data.
* Order-level details
* Product and customer keys
* Order, shipping, and due dates
* Sales amount, quantity sold, and price

### Initial queries explore the database structure using:

INFORMATION_SCHEMA.TABLES

INFORMATION_SCHEMA.COLUMNS

These help validate table creation and column definitions.

## Key Business Questions Answered

1. What countries do our customers come from?

2. What products are offered by category and subcategory?

3. What is the gender distribution of customers?

4. How many customers and products exist in the system?

5. What is the first and last recorded order date?

6. How many years of sales data are available?

7. Who are the youngest and oldest customers?

8. Computation of Sales Performance Metrics:
  * Total sales revenue
  * Total items sold
  * Average selling price
  * Total number of orders
  * Number of customers who have placed orders

9. Revenue & Distribution Analysis using:
  * Revenue by product category
  * Revenue by individual customer
  * Distribution of items sold across countries
  * Top 5 products by revenue
  * Bottom 5 products by sales quantity

10. Key Metrics Report: A consolidated KPI report is generated using UNION ALL, producing a single result set with showing:
  * Total Sales
  * Total Items Sold
  * Average Selling Price
  * Total Orders
  * Total Products
  * Total Customers
  * Customers Who Placed Orders
