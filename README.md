# LITA_CAPSTONE_PROJECT-Customer

###  Project Title : Smart Communication Customer Segmentation Analysis

[Project Overview](#Project-Overview)

[Data Source](#Data-Source)

[Tools Used](#Tools-Used)

[Data cleaning and Preparation](#Data-cleaning-and-Preparation)

[Exploratory Data Analysis](#Exploratory-Data-Analysis)

[Key Findings](#Key-Findings)

[Data Visualization](#Data-Visualization)

---
###  Project Overview
---
This is a data-driven project aimed at understanding and categorizing customers of Smart Communication based on their usage patterns,Service preferences, and demographic characteristics. By segmenting customers into distinct groups, Smart Communication can tailor its marketing, optimize product offerings, and enhance customer experiences through personalized communication.

###  Data Source
---
The Primary Source of Data used here is taken from customer Database of Smart Communication Limited.The Data provided is a table thats gives informations about the customers.
CustomerID,	CustomerName,	Region,	SubscriptionType,	SubscriptionStart,	SubscriptionEnd,	Canceled and Revenue	
![image](https://github.com/user-attachments/assets/43921a21-7e5c-4da9-bf35-a3e9b2526427)

###  Tools Used
---
- Microsoft Excel: For exploratory data analysis, summary statistics, and initial data cleaning.
   [Download here](https://1drv.ms/x/c/a7c3aecf7c2c74b7/EeAOvisv5DNEjzCCV82C-FQB6oBdZX01oafZ_V36Su7STw?e=8TP0Cx)
- Data Extraction & Preprocessing: Using SQL to extract and clean customer data from the database.
   [Download Here](https://1drv.ms/u/c/a7c3aecf7c2c74b7/ERZUG-x2swRGk7QZfJMaIPABJayToqHN4GjG9qDa7qQTKA?e=oBIXdf)
- Segmentation Analysis: Leveraging Power BI’s visualization and analytics capabilities to segment customers and identify insights within each segment.
- Github for portfolio building

###  Data cleaning and Preparation
---
Microsoft Excel and SQL were used for data cleaning tasks such as:
 -Handling missing values
 -Removing duplicates to ensure data integrity.
 -Standardizing data formats (e.g., date formats).
 -Transforming data types for consistency across the dataset.

I also applied some structured Query Language like

```Sql
   Select * from dbo.[[LITA Capstone_Customerdata]]]

   SELECT TOP 1 SubscriptionType, 
       COUNT(DISTINCT CustomerID) AS CustomerCount
FROM dbo.[[LITA Capstone_Customerdata]]]
GROUP BY SubscriptionType
ORDER BY CustomerCount DESC;

   SELECT SubscriptionType, 
       SUM(Revenue) AS TotalRevenue
FROM dbo.[[LITA Capstone_Customerdata]]]
GROUP BY SubscriptionType;

   SELECT 
    Canceled, 
    COUNT(*) AS TotalSubscriptions
FROM 
    dbo.[[LITA Capstone_Customerdata]]]
GROUP BY 
    Canceled;
```

###  Exploratory Data Analysis
---
This was done using Microsoft Excel and SQL to answer some salient questions needful for proper analysis. Important questions like

 o Analyze customer data using pivot tables to find subscription patterns.
 o Calculate the average subscription duration and identify the most popular 
   subscription types.
 o Create any other interesting report

 o retrieve the total number of customers from each region.
 
 o find the most popular subscription type by the number of customers.
 
 o find customers who canceled their subscription within 6 months.
 
 o calculate the average subscription duration for all customers.
 
 o find customers with subscriptions longer than 12 months.
 
 o calculate total revenue by subscription type.
 
 o find the top 3 regions by subscription cancellations. 
 
 o find the total number of active and canceled subscriptions.
