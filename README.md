# Capstone-Sales-Data-Project
This is my Project work on Sales Capstone Dataset as a Data Analysis student with Incubator Hub.

### Project Title: Sales Performance Analysis for a Retail Store
---

### Project Summary
---
This project is tasked with analyzing the sales performance of a retail store from January 2023 to August 2024. 
We will use the sales data to uncover key insights such as top-selling products, regional performance, and monthly sales trends. 
The goal is to produce an interactive Power BI dashboard that highlights these findings.

### Sources of Data 
---
The main source of the Data used is LITA Capstone Dataset .xls and it was transform to SalesData csv. for easy import to SQL.

### Required Tools
---
- Microsoft Excel
   1. For Data Cleaning
   2. For Analysis
   3. For Data Visualization
      
- SQL - Structured Query Language for Querying of Data
  
- Power BI
  1. For Business Intelligence reports
  2. For Data Visualization
 
 ### Data Cleaning and Preparations
  ---
  During the time of working on the Data, we perform the following action to cleaning and prepare the reports;
   1. Handling missing variables
   2. Data loading and Inspection
   3. Data Cleaning and formatting
 
### Exploratory Data Analysis
  ---
  Using EDA to answer some questions about the Data such as;
- Excel:
    1. Calculate metrics such as average sales per product and total revenue by region.
    2. Use pivot tables to summarize total sales by product, region, and month.

- SQL: Write the following queries to extract key insights based on the following questions; 
    1. retrieve the total sales for each product category.
    2. find the number of sales transactions in each region.
    3. find the highest-selling product by total sales value.
    4. calculate total revenue per product.
    5. calculate monthly sales totals for the current year.
    6. find the top 5 customers by total purchase amount.
    7. calculate the percentage of total sales contributed by each region.
    8. identify products with no sales in the last quarter.
  
### Data Analysis
  ---
  These are some of the lines of queries used during the process of analysing the Dataset;

```EXCEL
=SUMIF(C2:C9922,"Gloves",H2:H9922)
```

```EXCEL
=AVERAGEIF(C2:C9922,"Gloves",H2:H9922)
```

```SQL
SELECT * FROM [dbo].[SalesData_Project]
```
  
 ```SQL
 SELECT Product, SUM(Sales) as TotalSales
 from [dbo].[SalesData_Project]
 Group by Product
 ```

```SQL
SELECT Region,SUM(Sales) as Total_Sales
FROM [dbo].[SalesData_Project]
Group by Region
```

### Data Visualization

**EXCEL**

![Sales Data Excel 1](https://github.com/user-attachments/assets/221d00e4-dc9b-40f5-bc12-6cf7a05d222e)

![Sales Data Excel 2](https://github.com/user-attachments/assets/05239ce9-182b-4cfa-af36-e7458682cad8)

**SQL**




![My Project Sales Data 1](https://github.com/user-attachments/assets/4869f4cf-fbe7-443e-82f4-1ad6cc5f8d17)

![My Project Sales Data 2](https://github.com/user-attachments/assets/eacbdc11-7bb1-418f-bfea-010d8346f84d)


