# Avacados2Go
ETL Pipeline for an e-commerce app

Implemented a data warehouse for a retail company after interviewing the required stakeholders, gathered the business requirements, designed the data warehouse using SQL Server, performed ETL process using VisualStudio SSIS, and finally, valuable insights were derived using PowerBI dashboards.

## Business Use Case:
**Avocados2Go** is a retail organisation that:

* Sells all types of merchandises
* Acts as a broker for farmers by reselling their goods.
* Holds multiple branches across the country.

## Stakeholder Interview Questions:
1. What is the end goal and the problem statements or pain points that you wish to solve?
2. What are the key performance indicators or metrics that will be needed for the data analysis?
3. What is the budget you wish to allocate for this project?
4. Do you wish to maintain the historical data along with the incremental data? If so, what is the period from which the data is expected to be loaded into the warehouse?

## Subsequent Steps:
1. **Warehouse Creation:** We created the warehouse using SQL Server Management Studio.

2. **Pipeline Creation:** We created a simple ETL pipeline using SQL Server Integration Services.

3. **Integration with Power BI** We then integrated the SQL Server with Power BI for building visualizations.

4. **Report Generation:** We created multiple dashboards for retrieving actionable insights.

Separate reports for the aforementioned steps are included in separate folders under the same name.

## Conclusion:

We created the following dashboards:

![Dashboard 1](/Diagrams/Dashboard_1.png)

The dashboard showcases the decline in Sales through the ‘Sales over the Years’ graph. Moreover, we have forecasted the observed Sales trend to identify that, in the year 2022, there would be an increase in Sales followed by a steady Sales in 2023. 

The Dashboard also helps investigate the decline by offering: 

1. A Product Category deep-dive that shows which product category contributed most to the decline.

2. It also views Sales over the years through a Customer Lens through the ‘Sales by Name’ graph thus pointing out that the customer, Dominic, exhibits the biggest slump in sales.


![Dashboard](/Diagrams/Final_Dashboard.png)

This story-driven dashboard shows a clear pulse of the company's sales. By tracking the product performance over the years, sales by city, and forecast sales it’s easy to keep track of the performance.
The category wheat has the highest sales and the top three selling products have been Cinnamon Bread Loaf, Rotini, and Chocolate Chip Cookies. Avacodes2go has witnessed the highest sales in the year 2019. The forecasted sales price for 2022 is 3317. With the historical and predictive insights from the dashboard, the company can focus on ways to increase sales and profit.