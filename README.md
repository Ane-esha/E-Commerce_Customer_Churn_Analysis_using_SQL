## E-Commerce Customer Churn Analysis

- This project analyzes e-commerce customer data using MySQL to understand customer churn patterns, purchasing behavior, customer
  satisfaction, and retention trends. The dataset contains customer information, including tenure, preferred login devices, payment
   modes, city tiers, order categories, satisfaction scores, complaints, coupon usage, order counts, and cashback amounts.

-SQL queries were used to clean and transform the dataset, handle missing values and outliers, standardize inconsistent values, and 
perform exploratory data analysis. The project also explores the relationship between customer characteristics, shopping behavior, 
and churn status to identify insights that can help businesses improve customer retention and satisfaction.

# Project Objectives

- Clean the dataset by handling missing values and outliers.
- Standardize inconsistent categorical values.
- Transform existing columns and create new columns for better analysis.
- Analyze active and churned customer counts.
- Examine customer purchasing patterns, payment preferences, and coupon usage.
- Evaluate customer satisfaction and complaint patterns.
- Identify trends in order categories, cashback amounts, and customer behavior.
- Analyze customer return and refund information using SQL joins.

# Tools and Technologies

- MySQL: Data cleaning, transformation, querying, and analysis.
- MySQL Workbench: SQL query execution and database management.

# Project Workflow

1. Database and Table Creation

Created the database and imported the e-commerce customer dataset into a MySQL table containing customer attributes and purchasing 
information.

2. Data Cleaning

- Imputed missing numerical values using mean values.
- Filled missing categorical or discrete values using mode values.
- Removed records with "WarehouseToHome" values greater than 100.
- Standardized inconsistent values in login devices, order categories, and payment modes.

3. Data Transformation

- Renamed columns for consistency.
- Created "ComplaintReceived" to categorize customers based on complaint status.
- Created "ChurnStatus" to classify customers as Active or Churned.
- Removed the original "Churn" and "Complain" columns after creating the replacement columns.

4. Exploratory Data Analysis

Used SQL aggregate functions, filtering, grouping, sorting, subqueries, and conditional expressions to investigate:

- Active versus churned customers.
- Average customer tenure and total cashback amounts.
- Complaint percentages among churned customers.
- Customer distribution by city tier and gender.
- Preferred payment modes and order categories.
- Coupon usage and registered devices.
- Customer satisfaction scores and app usage.
- Average cashback by preferred order category.

5. Customer Returns Analysis

Created a separate "customer_returns" table containing return IDs, customer IDs, return dates, and refund amounts. 
Used SQL joins to combine return information with customer records and identify customers who had churned and submitted complaints.

# Key SQL Concepts Used

- "SELECT" and "WHERE"
- "UPDATE" and "ALTER TABLE"
- "CASE" statements
- Aggregate functions: "SUM()", "AVG()", "COUNT()", "MAX()", and "MIN()"
- "GROUP BY" and "HAVING"
- "ORDER BY" and "LIMIT"
- Subqueries
- "INNER JOIN"
- Data cleaning and column transformations

# Conclusion

This project demonstrates the use of MySQL for data cleaning, transformation, and exploratory analysis of e-commerce customer data. 
By examining churn status alongside customer satisfaction, complaints, purchasing preferences, and return information, the 
analysis helps identify customer behavior patterns that businesses can investigate when developing customer retention strategies.

The project also demonstrates practical SQL skills, including data manipulation, aggregation, conditional logic, subqueries, and joins, 
through a real-world business analysis scenario.
