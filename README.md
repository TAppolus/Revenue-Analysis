# Revenue-Analysis
This project analyses sales performance across product categories(Beauty,Clothing and Electronics

Retail Sales Data Analysis - SQL Query Documentation
Overview
This repository contains SQL queries for analyzing retail sales transaction data. The primary query extracts daily customer activity metrics with comprehensive date dimension breakdowns.
Dataset Schema
The analysis uses a retail sales dataset with the following structure:
Transaction ID: Unique identifier for each transaction
Date: Transaction date
Customer ID: Unique customer identifier
Gender: Customer gender (Male/Female)
Age: Customer age
Product Category: Category of purchased product (Beauty, Electronics, Clothing)
Quantity: Number of items purchased
Price per Unit: Unit price of the product
Total Amount: Total transaction amount


select COUNT(DISTINCT `Customer ID`)AS unique_customers,--i am counting different customers in my table
Date,
YEAR(Date) AS trans_year,--Extract the year from the date column

MONTH(Date)AS trans_month,--Extract the month from the date column
MONTHNAME(Date) as trans_month_name,

DAY(Date)AS trans_day,--Extract the day from the date column
DAYNAME(Date) as trans_day_name,--Extract the day name from the date column
