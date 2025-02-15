Maven Pizza-Sales-Data-Analysis


This Maven Pizza Sales Analysis project demonstrates proficiency in using SQL and Power BI to analyze and visualize data effectively, to uncover actionable insights into sales trends and product performance for a pizza restaurant.

PROBLEM STATEMENT


A popular maven pizza store wants to optimize its sales and marketing strategies to increase revenue and customer satisfaction.To achieve this, the company needs to analyze its sales data to uncover insights into customer preferences, sales trends, and product performance.The goal is to uncover insights from the data and develop actionable recommendations to drive business growth. The Client divided the problem statement into two sections;

KPI’s requirement


We need to analyze the key indicators for our Pizza sales data to gain insights into our business performance, we want to calculate the following metrics :

•	Total Revenue
•	Total Orders
•	Average Order Value
•	Total Pizzas Sold
•	Average Pizzas Per Order


Charts requirement We would like to visualize various aspects of our Pizza sales data to gain insights and understand key trends. We have identified the following requirements for creating charts :


•	Daily trend for Total Orders
•	Monthly trend for Total Orders
•	Percentage of sales by pizza Category
•	Percentage of sales by pizza Size
•	Total pizzas sold by pizza Category
•	Top 5 best selling & Bottom 5 worst selling pizzas


OBJECTIVES


Conduct a comprehensive sales performance analysis for a pizza store using SQL queries and visualize the findings using Power BI. The objective is to gain insights into sales trends, revenue distribution, and top performing products to inform strategic decision-making and optimize sales strategies.

DELIVERABLES


1. SQL Queries:
   
• Extract and aggregate sales data from the pizza sales dataset to calculate key metrics such as total sales revenue, average order value, Total Orders.

• Analyze sales trends over time (hourly, daily, monthly) to identify peak sales periods and seasonal variations.

• Calculate sales performance metrics for individual products, including best-selling pizzas, popular pizza sizes, and revenue contribution by product category.

2. Power BI visualizations:

   
• Develop interactive dashboards and visualizations to present the analysis findings in a clear and visually appealing manner according to business requirement.

• Create line charts to visualize sales trends over time, with filters for different time periods.

• Generate pie charts to illustrate revenue distribution by product category and size, highlighting top-selling items and revenue contribution.

• Incorporate slicers and filters to allow users to dynamically explore the data and uncover insights based on their specific criteria and interests.



DATA UNDERSTANDING


1. Dataset description
Source : Kaggle

Format : .csv

There are 4 datasets which contain detailed information about pizza orders, including specifics about the pizza variants, quantities, pricing, dates, times, and categorization details. The data spans a period of one year, from January 2015 to December 2015.

2. Data structure
Data type : .csv
Tables : 4
Fields : 12
Records : 48,620
Data Span : Jan 2015 - Dec 2015
Source : Maven Analytics
#1 ‘pizzas.csv’ dataset

   rows : 97
   columns : 4

 
   •	pizza_id : A unique identifier linking to a specific name of the pizza. (PK)


   •	pizza_type_id : Links pizza_types dataset. (FK)


   •	size : Represents the size of the pizza (e.g., small, medium, large).


   •	unit_price : The cost of a single unit of the specific pizza variant.
#2 ‘pizza_types.csv’ dataset

   rows :  32 
   columns : 4


   •	pizza_type_id : A unique identifier. (PK)


   •	name : Specifies the name of the specific pizza variant ordered.


   •	Category : Indicates the category of the pizza, such as vegetarian, non-vegetarian, etc.


   •	Ingredients : Provides a list or description of the ingredients used in the pizza.
#3 ‘orders.csv’ dataset

   rows : 21350
   columns : 3


   •	order_id : A unique identifier for each order made, which links to multiple pizzas. (PK)


   •	date : The date when the order was placed.


   •	time : The time when the order was placed
#4 ‘order_details.csv’ dataset

rows : 48620
columns : 4

 
•	order_details_id : unique identifier for all the orders made. (PK)


•	order_id : Links ‘orders’ dataset. (FK)


•	pizza_id : Links ‘pizzas’ dataset. (FK)


•	quantity : The number of units of a specific pizza variant ordered within an order.


3. Data Quality Assessment

   
The datasets appears to be relatively clean, with no missing values or obvious data errors. However, further exploration may reveal outliers or inconsistencies that need to be addressed during data cleaning.


5. CRAFTING QUERIES

1. Measure KPI’s

   
To measure and analyze various aspects of pizza sales data to assess sales performance.

•	Total revenue generated from pizza sales ?

•	Total number of orders placed ?

•	Average Order Value ?

•	Total number of pizzas sold ?

•	Average pizzas per order ?

•	Total quantity sold from each pizza category ?

2. Sales trend
   
To analyze how sales of pizza products vary seasonally or over specific time period.

•	Find peak time hours based on total orders ?

•	Average number of pizzas ordered per day ?

•	Order trend based on days ?

•	Order trend based on months ?


3. Product popularity

   
To measure the popularity and demand for different pizza products.

•	Category-wise distribution of pizzas ?

•	Most expensive pizza ?

•	Top 5 best selling pizza based on Total Orders ?

•	Top 5 pizzas based on sales for each pizza category ?

•	Percentage of sales by pizza category ?

•	Percentage of sales by pizza size ?



5. INSIGHTS

   
• FRIDAYS, THURSDAYS and SATURDAYS have the highest sales volume, comprising about 47% of total weekly sales, while Sundays and Tuesdays are typically slower days with lower sales.


• The busiest hours for pizza orders are between 12:00 PM to 1:00 PM and 5:00 PM to 6:00 PM, indicating high demand during lunch time and evening time.


• Peak sales occur during the SECOND QUARTER of the year and JULY being the month with highest sale.


• LARGE-sized pizzas are the most popular choice among customers, representing about 46% of total sales, followed by MEDIUM (30%) and SMALL (22%) sizes.


• Percentage share of total sales by all four Pizza Categories are almost same with CLASSIC category being the highest followed by SUPREME category.

• Among pizzas, THAI CHICKEN PIZZA contributes to maximum sales while CLASSIC DELUXE PIZZA are the most ordered one among the customers and BRIE CARRE PIZZA holds the position of least favoured pizza.

