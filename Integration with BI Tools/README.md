# Integrating the warehouse with Power BI

As we move onto the next stage of the Data warehousing for Avacados2Go, we would now be integrating the warehouse to Business Intelligence tools that help fully leverage the usage of data warehouses and help investigate and retrieve more actionable insights for the business. 

For these purposes, the BI Tool: **Power BI Desktop** was chosen as this was free and readily available on the internet. The installation was also self-explanatory and simple.

Once installed, for initial testing purposes, we connected to a sample employment statistic worksheet that encapsulates the employment numbers over the years. Once we connected and imported the dataset into Power BI, we noticed that employed numbers were abbreviated in thousands (like 1.5K) and therefore needed cleaning. We understood that such inconsistencies need to be addressed and cleaned at the ETL stages itself. 

We then created a sample line chart visualization for the worksheet using the automatically created Date Hierarchy and employment numbers. After playing around with the features, we also forecasted for the current trend of employment numbers and adjusted it to factor in the seasonality constraints. A similar chart was created for unemployment rates as well.

Moving forward, we successfully connected the data warehouse to the BI Tool and created a few derived attributes as columns in the Data pane for better visualizations. We then used these fields to create a Dashboard that showcases the sales over the years using the historical data, forecast over the following years and provides actionable insights to the business. 

![Power BI Integration](/Diagrams/Power_BI_Integration.png)