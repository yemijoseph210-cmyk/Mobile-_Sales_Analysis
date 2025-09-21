# Mobile_Sales_Analysis_

## An Overview:
+ This is a report on Mobile Sales

  ---

## Contents

---
### Project Overview:
"In this project, I analyzed mobile sales product data to uncover key insights on sales distribution across various attributes, including brand, customer gender, and payment method. Using pivot tables, I explored metrics such as:

- Sales by gender
- Sales by body style and annual income
- Sales by gender and annual income
- Sales by region and body style
- Sales by gender and color
- Sales by region "

This analysis provides valuable insights into the factors driving sales, enabling informed decision-making and strategic business planning

## Data Source:
www.kaggle.com/dataset

## Tools Used:
+ Pivot Table / Chart
+ Power BI
+ SQL


## Table Outlay:
First Three Colums

│Car_id │Date	│Customer Name	│Gender	│Annual Income	│Dealer_Name	│Company	│Model	│Engine	│Transmission	│Color	│Price ($)	│Dealer_No	│Body Style	│Phone	│Dealer_Region│
│----│----│----│----│----│----│----│----│-----│----│----│----│----│----│----│----│
│C_CND_000001	│02/01/2022	│Geraldine	│Male	│13500	│Buddy Storbeck's Diesel Service Inc	│Ford	│Expedition	│DoubleÃ‚Â Overhead Camshaft	│Auto	│Black	│26000	│06457-3834	│SUV	│8264678	│Middletown│
│C_CND_000002	│02/01/2022	│Gia	│Male	│1480000	│C & M Motors Inc	│Dodge	│Durango	DoubleÃ‚Â Overhead Camshaft	│Auto	│Black	│19000	│60504-7114	│SUV	│6848189	│Aurora│
│C_CND_000003	│02/01/2022	│Gianna	│Male	│1035000	│Capitol KIA	│Cadillac	│Eldorado	│Overhead Camshaft	Manual	│Red	│31500	38701-8047	│Passenger	│7298798	│Greenville│

# Query Languages (SQL)

Some of the Query Language to retrieve records are displayed here
``` SQL
---Categorise data into gold, silver and Diamond---
CASE
WHEN Price <= 500 THEN 'Silver'
WHEN Price <= 900 THEN 'Gold'
ELSE 'Diamond'
END AS Category
FROM[dbo].[mobile_sales];
```
---Retrieve the most expensive brand---
SELECT * FROM [dbo].[mobile_sales]
SELECT MAX(Price) AS 'Expensive Brand' FROM [dbo].[mobile_sales]
ORDER BY [Expensive Brand] DESC;
```












