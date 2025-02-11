# Online retail customer segmentation

## Data description
**This is a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.**  
- `InvoiceNo`: Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'c', it indicates a cancellation. 
- `StockCode`: Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.
- `Description`: Product (item) name. Nominal.
- `Quantity`: The quantities of each product (item) per transaction. Numeric.	
- `InvoiceDate`: Invoice Date and time. Numeric, the day and time when each transaction was generated.
- `UnitPrice`: Unit price. Numeric, Product price per unit in sterling.
- `CustomerID`: Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer.
- `Country`: Country name. Nominal, the name of the country where each customer resides. 

## Goals
- Convert data from being stored for each transaction to be data for each customer, and add valiable info of the customer
- Group customers to different clusters
- Analyze each cluster to identify unique charactaristics

## Converted data description
**It has 4372 rows, 13 columns**   
- `CustomerID` (Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer)
- `TotalOrders`(The number of orders for each customer, the cancelation is not included)
- `TotalSpent` (Total amount spent for each customer)
- `AverageValue`(average order value)
- `ItemsBought` (The number of items bought for each customer)
- `CanceledInvoices` (The number of cancelations for each customer)
- `MostFrequentDay` (Mode day for each customer)
- `MostFrequentHour` (Mode hour for each customer)
- `ProductDiversity` (Count of unique products purchased)
- `FirstPurchase` (The date of the first purchase)
- `LastPurchase` (The date of the first purchase)
- `Country` (Country name. Nominal, the name of the country where each customer resides)
- `LifeTime` column (The time differnce between first and last purchase, in number of days)
- `Recency` column (The time since the last purchase for each customer, in days)






## Questions to ask
- What are the main charactaristics of each cluster
- Whiche clusters have the highest value (Total amount spent over time)