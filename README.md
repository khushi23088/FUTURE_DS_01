E-Commerce Sales Dashboard (2011-2015)

This repository contains the code and resources for an E-Commerce Sales Dashboard covering the years 2011-2015. The dashboard provides a visual representation of sales data, including total sales, quantity, discounts, profits, and breakdowns by region, product, ship mode, and city over time. It utilizes DAX (Data Analysis Expressions) for advanced data modeling and calculations.

Overview

Total Sales: 2.30M

Total Quantity: 38K

Total Discount: 1.56K

Total Profit: 286.40K (with a minimum of 572.79K)


Visualizations

Sum of Discount by Region: Pie chart showing discount distribution across Central, East, West, and South regions.

Sum of Profit: Gauge chart indicating the total profit.

Sum of Sales by Ship Mode: Pie chart displaying sales distribution across Standard Class, Second Class, First Class, and Same Day shipping.

Sum of Sales by Product Name: Bar chart showing sales for various products.

Sum of Profit by Year and City: Line chart tracking profit trends for Detroit, Los Angeles, New York City, San Francisco, and Seattle from 2011 to 2015.


Categories

Furniture

Office Supplies

Technology

DAX Calculations
The dashboard leverages DAX to enhance data analysis:

Total Sales Calculation: TOTAL_SALES = SUM(Sales[Sales Amount])

Total Profit Calculation: TOTAL_PROFIT = SUM(Sales[Profit])

Discount Percentage: DISCOUNT_PCT = DIVIDE(SUM(Sales[Discount]), SUM(Sales[Sales Amount]), 0)

Yearly Growth: YEARLY_GROWTH = CALCULATE([TOTAL_SALES], PREVIOUSYEAR('Date'[Date]))

Regional Profit Share: REGIONAL_PROFIT_SHARE = DIVIDE([TOTAL_PROFIT], CALCULATE([TOTAL_PROFIT], ALL('Region')), 0)


These DAX measures enable dynamic filtering, aggregations, and time intelligence within the dashboard.
