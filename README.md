🛒 Zepto E-commerce SQL Data Analyst Portfolio Project

This is a real-world Data Analyst portfolio project built using an e-commerce inventory dataset from Zepto, one of India’s fastest-growing quick-commerce platforms.

The project simulates how data analysts work in real business environments, from raw data exploration to generating actionable insights using SQL.

🎯 Who This Project Is For

           📊 Data Analyst aspirants building strong portfolio projects

	       📚 Anyone learning SQL through real datasets

           💼 Candidates preparing for interviews in retail, e-commerce, or product analytics


📌 Project Objective

The goal is to replicate real-world analytics workflows used in e-commerce and retail businesses by:

        •	Setting up a messy, real-world inventory database
        
        •	Performing Exploratory Data Analysis (EDA)
        
        •	Cleaning inconsistent and invalid data


     Writing business-focused SQL queries to uncover insights related to:

        o	Pricing
        
        o	Inventory
        
        o	Stock availability
        
        o	Revenue potential


📁 Dataset Overview

The dataset is sourced from Kaggle and originally scraped from Zepto’s official product listings:

                   🔗 https://www.kaggle.com/datasets/palvinder2006/zepto-inventory-dataset/data?select=zepto_v2.csv

Each row represents a unique SKU (Stock Keeping Unit).

The same product may appear multiple times due to different sizes, weights, or pricing variations—just like real e-commerce catalogs.

🧾 Columns Explained

    •	sku_id – Unique product identifier (Primary Key)

    •	name – Product name

    •	category – Product category (Fruits, Snacks, Beverages, etc.)

    •	mrp – Maximum Retail Price (converted from paise to ₹)

    •	discountPercent – Discount percentage

    •	discountedSellingPrice – Final selling price in ₹

    •	availableQuantity – Stock count

    •	weightInGms – Product weight in grams

    •	outOfStock – Boolean value for availability

    •	quantity – Units per package


🔧 Project Workflow

1. Database & Table Creation
   
Created a structured SQL table with appropriate data types:

                CREATE TABLE zepto (
                
                  sku_id SERIAL PRIMARY KEY,
                  
                       category VARCHAR(120),
                  
                  name VARCHAR(150) NOT NULL,
                  
                       mrp NUMERIC(8,2),
                  
                  discountPercent NUMERIC(5,2),
                  
                       availableQuantity INTEGER,
                  
                  discountedSellingPrice NUMERIC(8,2),
                  
                     weightInGms INTEGER,
                  
                  outOfStock BOOLEAN,
                  
                  quantity INTEGER
                  
                );



2. Data Import

•	Imported the CSV file using MySQL tools

•	Ensured proper encoding (UTF-8)



3. 🔍 Data Exploration
   
•	Counted total records

•	Reviewed dataset structure

•	Checked for missing or null values

•	Identified unique product categories

•	Compared in-stock vs out-of-stock products

•	Found duplicate products across multiple SKUs



4. 🧹 Data Cleaning

•	Removed rows with zero MRP or selling price

•	Converted pricing values from paise to rupees

•	Standardized inconsistent data formats



5. 📊 Business Insights
   
•	Identified top 10 best-value products based on discounts

•	Found high-MRP products currently out of stock

•	Estimated potential revenue per category

•	Filtered premium products (₹500+) with low discounts

•	Ranked top 5 categories with highest average discounts

•	Calculated price per gram for value comparison

•	Grouped products into Low, Medium, and Bulk weight categories

•	Measured total inventory weight per category



🛠️ How to Use This Project


1️⃣ Clone the Repository

                    https://github.com/ShakilHossen537/E-commerce-Zepto--_SQL_data_analysis_project.git


2️⃣ Open the SQL File

zepto_SQL_data_analysis.sql includes:

        •	Table creation
        
        •	Data exploration
        
        •	Cleaning steps
        
        •	Business queries
        

3️⃣ Load the Dataset

•	Create a database

•	Run the SQL file

•	Import the dataset (UTF-8 encoding recommended)



📜 License

MIT License — feel free to fork, star ⭐, and use it in your portfolio.


👨‍💻 About the Author

Hi, I’m Md Shakil Hossen, a Data Analyst and SEO Specialist.
I simplify complex data problems and turn them into practical insights that help people learn, grow, and get hired.

🚀 Stay Connected

📺 Instagram
https://www.instagram.com/shakil_seo_expert/

Quick SQL tips, analytics content, and behind-the-scenes learning

💼 LinkedIn
https://www.linkedin.com/in/md-shakil-hossen-seo-specialist/

Let’s connect and grow professionally

