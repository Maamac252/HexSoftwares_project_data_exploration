# HexSoftwares_project_data_exploration
In this project at HEXASOFWARES, i preproccessed data with immense cleaning and removing inconsistency in the data. I explored and analyzed the dataset in a statistical approach. finally presented as bar charts, line charts and so on.
# Data Analysing using SQL
#Dataset source ( it was my own dataset about Gorgor Elecronic Sales 2023) with 366 rows and 7 columsn added 3 statsictical columns
#GOALS OF THIS PROJECT
- Which month the revenue increases
- The top customers who consumes our products
- Analyse reveneu trend over time
- the most generated revenue by product
  
all my work querries.sql
  
SELECT (price*quantity)AS total_sales_each_product,
product, order_date
FROM  [mydatabase].[dbo].[sales_data_500]
ORDER BY
total_sales_each_product DESC

 SELECT DISTINCT(order_id)
   FROM [mydatabase].[dbo].[sales_data_500]
   SELECT LEN(Price) AS leng_price
FROM  [mydatabase].[dbo].[sales_data_500]
ORDER BY 
price DESC

SELECT LEN(quantity) AS length
FROM  [mydatabase].[dbo].[sales_data_500]
ORDER BY
quantity DESC

SELECT COUNT(quantity) AS Quantity_count
FROM  [mydatabase].[dbo].[sales_data_500]

SELECT AVG(quantity*price) AS average_sale_of_all_products
FROM  [mydatabase].[dbo].[sales_data_500]
SELECT MAX(quantity*price) AS max_sales_of_all_products
FROM  [mydatabase].[dbo].[sales_data_500]
WHERE YEAR(order_date) = 2023
AND MONTH(order_date) = 1




 


SELECT SUM(price*quantity) AS sum_of_sales_all_products
FROM [mydatabase].[dbo].[sales_data_500]

SELECT 
    SUM(price * quantity) AS total_sales_january
FROM [mydatabase].[dbo].[sales_data_500]
WHERE YEAR(order_date) = 2023 
  AND MONTH(order_date) = 1

  SELECT 
  SUM(price*quantity) AS total_sales_Feb
  FROM [mydatabase].[dbo].[sales_data_500]
  WHERE YEAR(order_date) = 2023
  AND MONTH(order_date) = 2

  SELECT SUM(price*quantity) AS total_sales_march
  FROM [mydatabase].[dbo].[sales_data_500]
  WHERE YEAR(order_date) = 2023
  AND MONTH(order_date) = 3
   SELECT SUM(price*quantity) AS total_sales_April
  FROM [mydatabase].[dbo].[sales_data_500]
  WHERE YEAR(order_date) = 2023
  AND MONTH(order_date) = 4
   SELECT SUM(price*quantity) AS total_sales_may
  FROM [mydatabase].[dbo].[sales_data_500]
  WHERE YEAR(order_date) = 2023
  AND MONTH(order_date) = 5
   SELECT SUM(price*quantity) AS total_sales_june
  FROM [mydatabase].[dbo].[sales_data_500]
  WHERE YEAR(order_date) = 2023
  AND MONTH(order_date) = 6
  SELECT SUM(price*quantity) AS total_sales_july
  FROM [mydatabase].[dbo].[sales_data_500]
  WHERE YEAR(order_date) = 2023
  AND MONTH(order_date) = 7
   SELECT SUM(price*quantity) AS total_sales_AUG
  FROM [mydatabase].[dbo].[sales_data_500]
  WHERE YEAR(order_date) = 2023
  AND MONTH(order_date) = 8
   SELECT SUM(price*quantity) AS total_sales_Sep
  FROM [mydatabase].[dbo].[sales_data_500]
  WHERE YEAR(order_date) = 2023
  AND MONTH(order_date) = 9
   SELECT SUM(price*quantity) AS total_sales_Oct
  FROM [mydatabase].[dbo].[sales_data_500]
  WHERE YEAR(order_date) = 2023
  AND MONTH(order_date) = 10
   SELECT SUM(price*quantity) AS total_sales_NOV
  FROM [mydatabase].[dbo].[sales_data_500]
  WHERE YEAR(order_date) = 2023
  AND MONTH(order_date) = 11
   SELECT SUM(price*quantity) AS total_sales_DEC
  FROM [mydatabase].[dbo].[sales_data_500]
  WHERE YEAR(order_date) = 2023
  AND MONTH(order_date) = 12
