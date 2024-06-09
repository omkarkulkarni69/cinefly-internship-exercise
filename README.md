# cinefly-internship-exercise
  
## Project Description
This repository contains Walmart Sales Analysis Dashboard created for the final round interview at Cinefly. The dashboard offers insights into weekly sales performance by stores and sales trends found in the dataset.

## Key Objectives
- Develop a basic dashboard interface with essential visualizations.
- Analyze average weekly sales by store and holiday flag.
- Visualize sales trends over time.

## Setup Instructions
1. Clone the repository.
2. Run data preparation python notebook for dataset description.
3. Open the dashboard file in Power BI.

## Usage
- Run `Walmart_sales_preprocessing.ipynb` for dataset description.
- Open `Walmart_sales_analysis_final.pbix` in Power BI to view the dashboard.

## Data Preprocessing
1. After loading the dataset in Power BI, I extracted Month name and Year from the 'Date" column.
2. Ran a query to get Week Number (like week 1, week 2 etc) from the Date in a new column titled 'Week Number'.
3. Ran a query on Holiday_Flag to get description of presence of holidays (like No Holidays Week and Holiday Weeks) in a new titled 'HolidayDescription'.
4. Converted the Datatype of 'Weekly_Sales' into Accounting units (US Dollars) and rounded it to two decimal points.
5. Converted the Datatype of 'Fuel_Price' into Accounting units (US Dollars) and rounded it to two decimal points.
6. Rounded the decimal points of 'Temperature', 'CPI' and 'Unemployement' to two, three and three decimal points respectively.

## Methodology
1. Used Insert Shape to add a rectangle at the top of dashboard to add the title.
2. Added a card from visualization to display Total Yearly sales for one year.
3. Added a stacked column chart with Week Number on X-axis, Sum of weekly sales on Y-axis and Holiday Description in the Legend. After proper filtering and formatting, it displays Weekly Sales with columns coloured blue for weeks without holidays and red for weeks with holidays for the year 2010.
4. Repeated steps 7 to 9 twice to get results for 2011 and 2012.
5.  Created 3 buttons (one for each year) and assigned appropriate bookmarks to show only the results for the year selected on pressing the button.
6.  Added a Slicer with 3 years to have interactive visuals of YoY Sales Analysis, Seasonality Analysis and Yearly Sales by Store Analysis.
7.  Added a line chart Week Number on X-axis, Weekly Sales on Y-axis and Years on the Legend. This visual compares weekly perfromace of a particular store by year.
8.  Added a Treemap to get storewise contribution per year for the total sales of that year.
9.  Added a YoY Sales Analysis to show a store's 3 year sales analysis showing contribution of sales on Holiday weeks to the total yearly sales contribution.
10.  Added a button to add a pannel with slicers to add the buttons for three years and slicers for store numbers.
11.  Added another card which works with all the slicers to show average weekly sales.
12.  Formating and filtering done to make the dashboard visually apealling.

## Future Scope Work
1. Implementing a relationship between other parameters with the weekly sales.
2. The dataset is from the period 05-02-2010 to 26-10-2012. Trying forecasting and backcasting for the missing data like Straight Line Method or Linear Interpolation.
3. Optimizing the sales figures for the situations where sales from start of a year were included in the last week of previous year by dividing the sales data for 7 days and keeping the sales accurate for each week and month.  
