# Superstore-Sales-Analysis

![super](https://github.com/ashishwankhade0011/Superstore-Sales-Analysis/assets/160989632/fc227e3f-32b2-47f1-ae35-cba7d4bb013d)


# Introduction

In today's business landscape, data-driven decision-making is crucial for success. The Superstore Sales Analysis and Forecasting project leverages 
the power of data to uncover patterns, trends, and key insights within a sales dataset. By employing advanced analytics and visualization techniques,
this project assists stakeholders in understanding historical sales performance and predicting future trends.
# Process

# Data Preparation

The initial phase involved performing data cleaning tasks, including the removal of null values, the elimination of unnecessary columns,
handling duplicates, and adjusting data types to ensure data quality.

# Data Modeling

The subsequent step was to create calculated measures and tables using DAX (Data Analysis Expressions) in Power BI, enhancing the 
dataset's analytical capabilities

#Calculate a measure to determine the number of days it took for delivery.


  Days for shipment = DATEDIFF(SuperStore[Order Date],SuperStore[Ship Date],DAY)

#Created new columns to make easy calculations 


Month=Superstore[Order Date].[Month]


Quarter=Superstore[Order Date].[Quarter]


Year=Superstore[Order Date].[Year]


Day of week=WEEKDAY(Superstore[Order Date],2)


weekday/weekend=if(Superstore[Day of week]=6 || Superstore[Day of week]=7,"weekend","weekday")

# Data Analysis

Following data modeling, an in-depth data analysis was conducted within Power BI, utilizing various visualization techniques like matrices to 
identify trends in sales, region-wise sales, category-wise sales, and other pertinent insights.

# Dashboard Creation

The project proceeded with the development of an interactive and dynamic dashboard in Power BI. This dashboard was designed to include bookmark features,
allowing for seamless navigation between different charts and visualizations to provide a more comprehensive view of the data.

# Sales Forecasting

To deliver forward-looking insights, Power BI's advanced forecasting feature was utilized to perform a 10-day sales forecast. This forecasting capability
assists stakeholders in anticipating future trends and making informed decisions.

# Dashboard

The dashboard section offers an array of visualizations that empower users to explore and understand historical sales data. 
Key features of the dashboard include:

Visualization of monthly and yearly sales trends.


Comparison of sales across different categories and sub-categories.


Geographical distribution of sales.


Identification of top payment modes, segments, ship modes, and much more.




![dash1](https://github.com/ashishwankhade0011/Superstore-Sales-Analysis/assets/160989632/5fc46346-a858-42ac-9f94-bf08d4008e57)





