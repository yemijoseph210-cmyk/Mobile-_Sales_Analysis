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

│TransactionID│ Date│	MobileModel	Brand	Price	UnitsSold	TotalRevenue	CustomerAge	CustomerGender	Location	PaymentMethod
<img width="1153" height="30" alt="image" src="https://github.com/user-attachments/assets/d3a2362a-2bc7-4f58-b7ca-c2faa285a429" />

│----│----│----│----│----│----│----│----│-----│----│----│----│----│----│----│----│

TransactionID	Date	MobileModel	Brand	Price	UnitsSold	TotalRevenue	CustomerAge	CustomerGender	Location	PaymentMethod
79397f68-61ed-4ea8-bcb2-f918d4e6c05b	01/06/2024	direction	Green Inc	1196.95	85	28002.8	32	Female	Port Erik	Online
4f87d114-f522-4ead-93e3-f336402df6aa	04/05/2024	right	Thomas-Thompson	1010.34	64	2378.82	55	Female	East Linda	Credit Card
6750b7d6-dcc5-48c5-a76a-b6fc9d540fe1	2/13/2024	summer	Sanchez-Williams	400.8	95	31322.56	57	Male	East Angelicastad	Online
7da7de95-f772-4cc2-bce0-b0873f98233e	4/17/2024	keep	Greer and Sons	338.6	79	31159.75	46	Other	East Kevin	Cash
<img width="1057" height="146" alt="image" src="https://github.com/user-attachments/assets/cfb096c6-580c-46e3-9dfd-55d1afb7aa91" />

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
```SQL
---Retrieve the most expensive brand---
SELECT * FROM [dbo].[mobile_sales]
SELECT MAX(Price) AS 'Expensive Brand' FROM [dbo].[mobile_sales]
ORDER BY [Expensive Brand] DESC;
```












