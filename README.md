# Sales Analysis and Promotion Planning BI Initiative

## Overview

The project focuses on integrating various BI tools and methodologies to analyze sales data and generate insightful reports.

## Project Components

### I. SSRS Integration Project

1. **Data Flow Task**
   - Responsible for the extraction, transformation, and loading (ETL) of data for sales analysis.

2. **Data Sources and Destinations**
   - Illustrates the tables used for sales analysis, such as clients, categories, employees, distributors, and products.
   - Data is extracted from these tables and loaded into corresponding dimension tables in the destination database.

3. **Time Dimension**
   - SQL query generates the Time dimension from the data source, creating a table with columns for day, month, and year for time-based sales analysis.

4. **Fact Table: VentesRemise**
   - Combines data from OrderSrc and OrderDetailsSrc.
   - Uses components like Sort and Merge Join to combine data based on OrderID.
   - Result is loaded into the VentesRemise fact table, containing measures and foreign keys related to other dimensions (Time, Client, etc.).

### II. Multidimensional Analysis Project (SSAS)

- Created an OLAP cube with a star schema for sales analysis.
- Central fact table 'FactSales' is surrounded by several dimension tables.

### III. Multidimensional Queries

1. **Discounts by Client and Product**
2. **Discounts by Client, Product, and Category**
3. **Total Orders by Country**
4. **State with Maximum Sales in the USA**
5. **Product with the Highest Discount**
6. **Best and Least Sold Product by Country**
7. **Sales Percentage by Client and Country**
8. **Number of Sales per Year**

### IV. SSRS Reporting Project

1. **Report on Quantity Sold by Continent, Country, and City**
   - SQL query and results for visualizing sales by geographical regions.

2. **Report on Top-Selling Products by Country**
   - SQL query and results for visualizing the most sold products in different countries.

3. **Sales Trend by Country Over the Years**
   - SQL query and results for visualizing sales trends over time.

4. **Report on Top-Selling Products by Year**
   - SQL query and results for visualizing top-selling products based on yearly data.
