# Project Tile: Northwind-Traders Project

## Disclaimer: This is not real-world project but use for the purpose of learning to demostrate my skills in Excel and PowerBI

- title: Analysing Northwind-Trader data-set to answer business questions using Excel and powerBI
- author: Tosin Emmanuel
- Date: 2023-12-26

## Project Description

This is an analysis of the Sales performance of Northwind Traders, I will analyse data from Northwind Trader dataset from category table,customer table,employee table,order table,order_detail table,products table and shipper table both on Excel and powerBI to solve different business questions, I imported the dataset to excel and powerBI from local disk respectively.

## Problem Statement.

- The goal of this anlysis is to solve the following in Excel;
  - Calculate the total sales (revenue) for each category of products.
  - Determine which customer has placed the highest number of orders.
  - Calculate the total sales generated by each employee.
  - Show the trend in sales over time.
  - Calculate the average time it takes to process an order from the order date to the
shipped date.

- Also solve the following with PowerBI;
building a top-level KPI dashboard for the executive team. Its purpose should be to allow them to quickly understand the company's performance in key areas, including:
  - Sales trends
  - Product performance
  - Key customers
  - Shipping Cost

## Skills and Concept Demonstrated:

- Excel
  - pivot table
  - data modeling
  - functions:inedx,match,mode,average.
- PowerBI
  - creating new column to calculate total price
  - Creating key performance indicators (KPIs) and other business calculations,
  - Data modelling
  - using Dax to perform basic measures
  - filters
  - tooltips
  - Ccreating Dashboard

 ## Data Source

 The data used for this work is gotten from Northwin Traders. I studied the Schema, Objects related to the Schema, data dictionary and found the right tables for the analysis.

You can find a link to get started with installation and restoration of the database to your local machine. [here](https://maven-datasets.s3.amazonaws.com/Northwind+Traders/Northwind+Traders.zip)

## Data Transformation

- I added another column on orders table to calculate days between the order and the ship date
  ![image](https://github.com/AdebayoTosin/Northwind-Traders-Excel-and-PowerBI/blob/main/orders%20data%20modelling.png)
- After carefully studying the data set, I have to add column showing calculation for TotalPrice on Order_details Table, this is done in both excel powerBI
  ![image](https://github.com/AdebayoTosin/Northwind-Traders-Excel-and-PowerBI/blob/main/order_details%20transformation.png)
  ![image](https://github.com/AdebayoTosin/Northwind-Traders-Excel-and-PowerBI/blob/main/powerBI_data.png)

- I began writing several Dax with aggregate to create measures with right metrics. Measures  created name is "Measures".
![image](https://github.com/AdebayoTosin/Northwind-Traders-Excel-and-PowerBI/blob/main/dax%20measures.png)

## Data Modelling

Tables were automatically joined by creating relationships with them, PowerBI does this intelligently. However, as someone that understands the dataset and want to get specific insights and information. I had to desmostrate my skill inthis by removing the automation and did another model.

![image](https://github.com/AdebayoTosin/Northwind-Traders-Excel-and-PowerBI/blob/main/powerBI%20data%20modelling.png)

## Data Analysis and Visualization

- Calculate the total sales (revenue) for each category of products.
  - I used pivot table to calculate the sales revenue by creating relationship and joining categories table and order_details table
    ![image](https://github.com/AdebayoTosin/Northwind-Traders-Excel-and-PowerBI/blob/main/Revenue%20for%20product%20category.png)

- Determine which customer has placed the highest number of orders.
  - This is solved by using the combination of index,mode and match functions on customerID column Orders table.
    ![image](https://github.com/AdebayoTosin/Northwind-Traders-Excel-and-PowerBI/blob/main/customer%20with%20highest%20order.png)
    ![image](https://github.com/AdebayoTosin/Northwind-Traders-Excel-and-PowerBI/blob/main/customer%20with%20highest%20order%202.png)
 - Calculate the total sales generated by each employee.
   - I used pivot table to do this calculation by creating relationship and joining employee table and order_details table
![image](https://github.com/AdebayoTosin/Northwind-Traders-Excel-and-PowerBI/blob/main/revenue%20by%20employee.png)
- Show the trend in sales over time.
  - I used pivot table to join and create relationship betwee  Order table and order_details table. i show trends in  **sales in months history and sales over time**
![image](https://github.com/AdebayoTosin/Northwind-Traders-Excel-and-PowerBI/blob/main/month%20order%20history.png)
![image](https://github.com/AdebayoTosin/Northwind-Traders-Excel-and-PowerBI/blob/main/revenue%20over%20time.png)

- Calculate the average time it takes to process an order from the order date to the
shipped date.
  - average function is used on Order table days_btw_orderdate_shipdate column
![image](https://github.com/AdebayoTosin/Northwind-Traders-Excel-and-PowerBI/blob/main/Average%20days.png)

- PowerBI dashboard showing;
  - Sales trends
  - Product performance
  - Key customers
  - Shipping costs
  ![image](https://github.com/AdebayoTosin/Northwind-Traders-Excel-and-PowerBI/blob/main/PowerBI%20dashboard.png)

## Insight

- There are 8 categories of products and beverages has the highest revenue of $286,526.95
- CustomerID that place the highest order is SAVEA with 31 orders
- Employee with the highest sales generated is Margaret Peacock
- With the history of sales in months over 2013,2014,2015,there is highest order in March and April with 103 andd 105 orders respectively
- Overtime the highest revenue was genrated in 2015 April with 134,630.56
- The Average time it takes to process an order from the order date to shipped date is 8days
- The total shippingcost generated between 2013,2014,2015 is $64.94k
- There are 91 customer that generate 830 order i 21 countries over the years in the dataset
- Total revenue generate is $1.27m
- federal shipping has 20.51k shipping cost with 255 orders,
  speed express has 16.19k shipping cost with 249 orders,
  united package has 28.24k shipping cost with 326 orders

## Recommendation

There are no doubts that the Business is performing well as the sales is in up trend as the years progress. However there is room for more improvement.

- There just 91 customers in 21 countries that make 830 orders, there should be improvement in sale,advertisment and discount  to attract new customer
- The cost Shipping should be reduced to increase profit margins,the 3 shipping companines currently in use are cost effective than the other. federal shipping is expensive to use ,further investigation should be done to know why.
- Awards and incentive should be introduced among the employee to create competition that improve sales.
- There is reportedly  low sales in june of every year in the dataset, further investigation should be done to know why and solution should be provided to increase sale in this month and accross other month.

## Thank you for reading

I am open for entry-level data anlalyst role.

Let us have discussion about your company and industry now!








Welcome to my portfolio.
This project demostrate my skill in **Excel** and **PowerBI**


