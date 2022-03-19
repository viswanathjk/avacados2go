# Operational issues:
Currently, the organisation’s operation involves multiple issues and inconsistencies, some of which are:
1. Not all customer data is stored, only loyalty customer’s data are stored.
2. Excel is used for tracking and reporting purposes, containing primitive structure and data points.
3. No standard return policy.
4. Not tracking important metrics such Quantity and Discounts offered, thereby leading to incompetent and mostly incorrect analytics.
5. Inventory, Procurement Costs and Regional data are not stored.

# Requirements:
The organisation hopes to gain the following advantages from implementing a data warehouse:
1. Ability to store all customer’s data.
2. Tracking inventory for acquiring goods on time.
3. Storing data regarding discounts offered and procuring costs for accurate analysis.
4. Track sales revenue and make forecasts using accurate data.
5. Optimizing customer feedback loop for swift action.
6. Utilize the regional data stored to develop an appropriate action plan.

# Methodology:
Currently, the Kimball and Inmon methodologies are the most widely used architectures for designing a data warehouse. The choice between the two, however, depends on the organisation’s use case and what they wish to leverage from the data warehouse.

For Avocados2Go, a bottom-up approach such as the Kimball method would be a better fit. This is because their requirements are specific to improving certain business processes and the data format is preferred to be denormalized.

# Activities:
1. Eliciting business requirements and KPIs from the appropriate stakeholders.
2. Negotiating on a feasible budget.
3. Choosing an appropriate methodology for the data warehouse architecture.
4. Plot the Enterprise Bus Matrix based on the business processes.
5. Design dimensional model.
6. Platform selection.
7. Plotting roadmap.
8. Development.
9. Launch.

# Enterprise Bus Matrix:
![Enterprise Bus Matrix](/Diagrams/Enterprise%20Bus%20Matrix.png)

# Initial Dimensional Model:
![Dimensional Model](/Diagrams/Dimensional%20Model.png)

# Limitations:
The following are the potential limitations that the data warehouse may face in the future:
1. Lack of historical data regarding non-loyalty customers to spot trends.
2. Data warehouse maintenance.
3. Denormalized data can lead to data redundancy.
4. Current OTC type of discounts will lead to big problems.
5. Standard format should be followed.
6. Schematic enforcement will cause data loading issues.