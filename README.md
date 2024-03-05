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

# Category And Sub-Category Level
![dash2](https://github.com/ashishwankhade0011/Superstore-Sales-Analysis/assets/160989632/ae18ea39-a679-450e-b74b-c9dce399f034)


# Region And State Level
![dash3](https://github.com/ashishwankhade0011/Superstore-Sales-Analysis/assets/160989632/1969b889-21ff-477b-92e5-07f6c6a184d1)


# Sales Forecasting 

![dash4 sale](https://github.com/ashishwankhade0011/Superstore-Sales-Analysis/assets/160989632/293d9adc-b906-4ae2-9a2f-21f4eac489f7)

The sales forecasting page focuses on predicting sales for the subsequent 10 days. Leveraging historical sales data and
advanced forecasting techniques of Power BI.

# Key Insights
The dashboard and forecasting page unveil the following key insights:

Monthly Peaks: Noteworthy sales spikes in February, August, and October hint at recurring patterns.

Parallel Growth: While 2020 exhibits higher sales than 2019, the trend patterns remain consistent.

Geographic Leaders: California takes the lead in sales, closely followed by New York.

Region Impact: The West region contributes the most to overall sales.

Payment Preference: Cash On Delivery (COD) emerges as the preferred payment method.

Consumer Champion: The consumer segment generates the highest sales figures.

Top Category: Office Supplies stand out as the dominant sales category.

Preferred Shipping: Standard Class is the preferred shipping choice.

Sub-Category Stars: Phones and chairs emerge as the top-selling sub-categories.


# Tech Stack
Project relies on the following key technologies:

Power BI Desktop Design, visualization, and interactive reporting.
DAX (Data Analysis Expressions) Creation of calculations and measures supporting data visualizations.
Advanced Analytics Predict future sales trends based on historical data.
Power Query Clean and transform raw data into a structured format.





