Power BI Data Modeling Documentation
Project Overview
This documentation provides an overview of the data modeling process in Power BI. The project includes the creation of a conceptual and logical model, the development of a data model in Power BI, the design of a snowflake schema, data cleaning, and the addition of a date dimension table.

Project Components
Conceptual and Logical Model
A conceptual and logical model was created using Draw.io. The model includes the following tables:
FactSales
FactBudget
DimProduct
DimCustomer
DimCatSeg (Category and Segment)
DimDate
DimGeography
Data Model in Power BI
Two fact tables were created in Power BI:

FactSales
FactBudget
Four dimension tables were established:

DimProduct
DimCustomer
DimCatSeg (Category and Segment)
DimDate
DimGeography
Snowflake Schema
A snowflake schema was designed for the data model, providing a structured way to organize data tables and relationships. This schema facilitates efficient querying and reporting.
Data Cleaning
Data cleaning involved the transformation of the "Email Name" column, which was split into separate columns for "Email," "First Name," and "Last Name" using a delimiter.

Duplicate records within dimension tables were removed to maintain data integrity.

Date Dimension Table
A date dimension table was added to provide date-related attributes for time-based analysis. The table was generated using Power Query M code to create date attributes such as year, quarter, week number, month number, month name, and day of the week.
PowerQuery
Copy code
// Power Query M code to create the Date Dimension table
(StartDate as date, EndDate as date) => ...
Conclusion
The Power BI data modeling project successfully created a structured data model with fact and dimension tables, a snowflake schema, data cleaning, and a date dimension table. This model is now ready for use in generating insightful reports and visualizations.