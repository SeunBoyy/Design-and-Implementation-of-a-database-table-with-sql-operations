# Design-and-Implementation-of-a-Database-table-with-SQL-operations

## Project Overview
This project demonstrated the ability to design and create a database table, perform various SQL operations to manage and retrieve data. It showcases proficiency in sql syntax and database management.

## Data sources
The primary dataset used for this analysis is the "Product" dataset generated during the Analysis

## Tools used
- Excel - Data Cleaning 
- SQL- Writing queries

## Data Cleaning/Preparation
In the initial data-cleaning phase, I performed the following tasks;
- Data loading and inspection
- Data formatting

## Expository Data Analysis(EDA)- SQL
EDA involved exploring the sales data to answer key questions, such as;
- What are the details of the products available, including their names, prices, and quantities?
- What is the total salary earned by each employee, and how do they rank in terms of total earnings?
- What are the details of employees located in Abia state?

```SQL
CREATE TABLE PRODUCTS (PRODUCT_ID INT PRIMARY KEY IDENTITY(10,5),PRODUCT_NAME VARCHAR (50),QUANTITY_PRICE INT)

SELECT * FROM PRODUCTS

ALTER TABLE PRODUCTS
ADD QUANTITY INT

INSERT INTO PRODUCTS(PRODUCT_NAME,QUANTITY_PRICE,QUANTITY)
VALUES
('REFRIGERATOR', 800000,50),
('HOME THEATRE',350000,20),
('TV STAND',300000,10),
('OFFICE DESK', 500000,40),
('OX FAN',900000,60)

SELECT * FROM EMPLOYEE

SELECT EMP_NAME,SUM (EMP_SALARY)AS [SUM OF SALARY] FROM EMPLOYEE
GROUP BY EMP_NAME
ORDER BY [SUM OF SALARY] DESC

SELECT * FROM EMPLOYEE
WHERE STATE='ABIA'
```
## Review
The dataset provides a comprehensive overview of the products available within the organization, detailing their names, prices, and quantities. The structure of the dataset appears well-organized, facilitating easy access to essential information about each product.



























