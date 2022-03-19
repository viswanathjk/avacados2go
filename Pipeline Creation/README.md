# Creating a simple ETL pipeline

## Summary:

We first created the basic structure and the tables for the warehouse using the SQL server and SSMS. In the following report, we will be detailing the steps that we followed to fill the tables with the appropriate data to populate this data warehouse.

* In an effort to build the final production database for the organization, we tried importing a database in the form of a .bak file into the Server. However, we encountered errors owing to not storing the file in the appropriate file path. 

* We then accessed the SSMS  and accessed the locally running database server and restored the database provided. However, after restoring, we also faced two other challenges viz., the database diagrams were missing relationships and weren't accessible and required explicit public permission for access.

* Moving forward, we populated the Date dimension table for the organisation by writing and executing scripts, according to the defined caveats.

* We then manually added data by running an SQL Insert Query into the Customer dimension.

* We downloaded and installed Visual Studio along with the Data storage and processing capacity as this provides us with the inbuilt SSIS tool.

* After creating a SSIS project, we started our work on creating an ETL pipeline. The first step towards this involved creating a Data Flow task. This mandates the automated actions that needs to take place for the ETL pipeline. 

* We also set up the connection manager for setting the source and destination  of the ETL pipeline as the Excel files and localhost server.

* We then standardized the data types by altering the Excel files’ datatypes through Data Conversion.

* We then accessed the Slowly Changing Dimension Wizard to account for updation, deletion or creation scenarios to existing dimensions.

* Post this, we ran the ETL process successfully.

## Dimensional and Fact Tables
![Dimensional and Fact table 1](/Diagrams/Dim_and_Fact_1.png)
![Dimensional and Fact table 2](/Diagrams/Dim_and_Fact_2.png)