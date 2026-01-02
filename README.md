🛒 E-commerce Zepto – SQL Data Analysis Project
📌 Project Overview

This project focuses on data analysis using SQL based on an e-commerce dataset inspired by Zepto. The goal is to analyze product availability, pricing, and category-level insights using structured SQL queries.

The project simulates how real-world e-commerce platforms manage and analyze large datasets to support business decisions such as pricing strategy, inventory management, and product performance.

📂 Dataset Information

The project uses the dataset:

📄 zepto_v2.csv

This dataset contains information related to products available on the Zepto platform.

Key Attributes Include:

Product Name

Category

Price

Availability / Stock Status

Quantity / Weight

Other product-related details

This dataset is used to perform meaningful SQL-based analysis.

🎯 Project Objectives

Analyze product availability and pricing

Understand category-wise distribution

Practice SQL queries on a real-world dataset

Improve data analysis and problem-solving skills

Build a strong SQL portfolio project

🛠️ Tools & Technologies Used

SQL – Querying and data analysis

CSV Dataset – Data source

MySQL / PostgreSQL / SQLite – Database engines

🔍 Sample SQL Queries
1. View all products
SELECT * FROM zepto_v2;

2. Find products currently in stock
SELECT *
FROM zepto_v2
WHERE availability = 'In Stock';

3. List products by price (low to high)
SELECT product_name, price
FROM zepto_v2
ORDER BY price ASC;

4. Count total number of products
SELECT COUNT(*) AS total_products
FROM zepto_v2;

5. Category-wise product count
SELECT category, COUNT(*) AS total_products
FROM zepto_v2
GROUP BY category;

📊 Key Insights (Example)

Identified top product categories by availability

Analyzed pricing distribution across categories

Detected out-of-stock products

Improved understanding of inventory structure

🚀 Future Enhancements

Add customer and order datasets

Perform advanced analytics using JOINs

Create dashboards using Power BI or Tableau

Build a simple frontend interface

📁 Project Structure
E-commerce-Zepto--_SQL_data_analysis_project/
│
├── zepto_v2.csv
├── queries.sql
└── README.md
