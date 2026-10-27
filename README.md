# SQL-Repo
A place to put all of my sql projects.

# SQL Retail & Sales Data Analysis Project

## Overview
This project was completed as part of a **Data Technician Bootcamp** and demonstrates the use of **SQL** to query, analyse, and extract valuable business insights from retail and sales datasets. Working with relational databases, the project focused on retrieving, filtering, aggregating, and combining data to support business decision-making and reporting. Based on practical exercises using the Northwind database and other relational datasets, the project covered real-world sales, customer, product, and order analysis. 【1-772788】

## Key Skills Demonstrated

### Querying Data
- Writing SQL queries using:
  - `SELECT`
  - `WHERE`
  - `ORDER BY`
  - `GROUP BY`
  - `DISTINCT`
  - `BETWEEN`
  - `IN`
  - `LIKE`
- Extracting relevant business information from large datasets
- Filtering records based on specific business requirements
- Sorting and organising query results for reporting purposes

### Data Analysis
- Analysing customer, product, and sales data
- Identifying sales trends and product performance
- Performing customer segmentation and location-based analysis
- Generating summary statistics and aggregated reports
- Calculating product counts, sales volumes, and order metrics using aggregate functions

### Working with Relational Databases
- Understanding database structure and relationships
- Applying primary and foreign key concepts
- Designing and querying relational data models
- Combining data across multiple tables using SQL joins

### SQL JOINs
- Using `INNER JOIN` to combine related records across tables
- Working with supplier, product, category, customer, employee, and order data
- Creating comprehensive business reports from multiple data sources
- Understanding and applying:
  - INNER JOIN
  - LEFT JOIN
  - RIGHT JOIN
  - FULL OUTER JOIN
  - CROSS JOIN

## Retail & Sales Insights Explored

The project used SQL to answer business-focused questions such as:

- Which products generate the highest sales volumes?
- Which categories contain the most products?
- Which suppliers provide specific inventory items?
- Which customers placed orders during a selected period?
- How do sales vary across products and categories?
- Which products are considered high-value based on price?
- What trends can be identified from historical order data?

## Example SQL Techniques Used

```sql
SELECT CustomerName, City
FROM Customers
WHERE Country = 'UK'
ORDER BY CustomerName;
```

```sql
SELECT CategoryName,
       COUNT(ProductID) AS ProductCount
FROM Categories
JOIN Products
  ON Categories.CategoryID = Products.CategoryID
GROUP BY CategoryName;
```
```sql
SELECT Products.ProductName,
       Categories.CategoryName,
       Suppliers.SupplierName
FROM Products
JOIN Categories
  ON Products.CategoryID = Categories.CategoryID
JOIN Suppliers
  ON Products.SupplierID = Suppliers.SupplierID;
```
## Tools & Technologies

- SQL
- PostgreSQL / Supabase
- Relational Databases
- Northwind Database
- Data Analysis & Reporting
- Database Design
- Database Querying
- Data Aggregation & Filtering

## Learning Outcomes

Through this project, I developed practical experience in:

- Writing efficient SQL queries to retrieve and analyse business data
- Using `SELECT`, `WHERE`, `ORDER BY`, and `GROUP BY` statements to answer business questions
- Filtering and organising large datasets for reporting purposes
- Creating summary reports using aggregate functions such as `COUNT()`, `SUM()`, and `AVG()`
- Combining data from multiple tables using SQL JOINs
- Understanding and working with relational database structures
- Translating business requirements into data-driven SQL solutions
- Extracting actionable insights from retail and sales datasets

## Project Outcome

The project demonstrates practical SQL skills used in data analysis and business intelligence. By combining querying, filtering, aggregation, and table joins, I was able to transform raw retail and sales data into meaningful insights that support reporting, operational monitoring, and data-driven decision-making.
