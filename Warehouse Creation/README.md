# Installing a SQL Server and Creating a Warehouse

We first elicited the business requirements and KPIs from the stakeholders by interviewing them iteratively and designed a high-level dimensional model according to the same. We then set the right expectations, clarified the limitations, and conveyed the feasibility to the appropriate stakeholders.
 
## Initial Dimensional Model: Avacados2Go
![Initial Dimensional Model](/Diagrams/Dimensional%20Model.png)

However, based on the stakeholder’s suggestion, we realized that the Dimensional model required changes in terms of **Payment** and **Product** dimensions, owing to its many-to-one relationship with the **Sales** fact. Therefore, it was decided to make **Payment** a degenerate dimension and the **Dim_Payment_Type** was included in the **Sales** Fact table.

## Updated Dimensional Model: Avacados2Go
![Updated Dimensional Model](/Diagrams/Updated_Dimensional_Model.jpg)

Following this, we started creating the blueprint of the data warehouse in SQL Server. 

1.	Firstly, we successfully installed SQL Server Management Studio (SSMS) on our Windows machines.
2.	We then moved onto creating a database “MGS657_ALPHA_LAB” as a sample project.
3.	We then created tables for Employees and Store and a database diagram for the sample project. Screenshots of the same are attached below.
4.	Using this experience, we created the database “MGS657_Avacados2Go” database for the project.
5.	For this database, we started creating tables for both the Dimensions and Facts listed in the dimensional model.
6.	We created tables for the dimensions: Customer (Dim_customer), Employee (Dim_employee), Offers (Dim_offers), Products (Dim_product) and for Shops (Dim_shop).
7.	We also created a Fact table with Sales (Fact_Sales).
8.	Once done, we started mapping the relationships between the tables. Each of the relationships i.e., Sales and:

* Customer: FK_Sales_Customer_Customer_ID (PK_Customer_ID, FK_Customer_ID)
*	Employee:  FK_Sales_Employee_Employee_ID (PK_Employee_ID, FK_Employee_ID)
*	Offers: FK_Sales_Offer_Offer_ID (PK_Offers_ID, FK_Offer_ID)
*	Product: FK_Sales_Product_Product_ID (PK_Product_ID, FK_Product_ID)
*	Shipment: FK_Sales_Shipment_Shipment_ID (PK_Shipment_ID, FK_Shipment_ID)
*	Shop: FK_Sales_Shop_Shop_ID (PK_Shop_ID, FK_Shop_ID)
*	Date: FK_Sales_Date_Datekey (Date_key, FK_date_key)

9.	The screenshots of the Database diagram and Schema changes history are available in the attached report
