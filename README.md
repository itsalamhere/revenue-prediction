# revenue-prediction

## Revenue Prediction via Customer Lifetime Values

One of ways to indicate customer engagement in a certain period is by customer lifetime values (CLV). CLV consists of RFM analysis, which stands for Recency, Frequency, and Monetary Value. Other variables in the realm can also be extracted as supporting data, such as total quantity, purchase hour, average value and size, up to if a customer buys on the weekend. These data can be used to predict returning customers with their respective revenues for the store.

In this project, we'll be analyzing variables of customer behavior (RFM and its adjacent) to predict returning customers and their respective revenues. We will use a dataset of [Online Retail II](https://archive.ics.uci.edu/dataset/502/online+retail+ii) from UCI Machine Learning Repository. The dataset contains 2-year online retail transactions (01/12/2009 to 09/12/2011) with a total of 1,067,371 data. The columns consist of:

* `InvoiceNo` : Invoice Number; Code starting with 'C' indicates a cancellation,
* `StockCode` : Product (item) code; 5-digit integral number assigned to each distinct product,
* `Description` : Product (item) name,
* `Quantity` : The number of product (item) bought per transaction,
* `InvoiceDate` : Invoice date and time,
* `UnitPrice` : Product price per unit (in poundsterling),
* `Customer ID` : Customer number as identifier, and
* `Country` : Name of country where the customer resides.

The project will be divided into four main sections:
1. `01-EDA-and-data-cleaning`, where we'll be cleaning the data (missing values, duplicates, non-transactions),
2. `02-data-analysis-and-data-wrangling`, where we'll extract RFM values and visualize it as a whole and also by country,
3. `03-feature-engineering`, where we're extracting all CLV variables for the purpose of revenue prediction, and
4. `04-revenue-prediction`, where we're finding the best model of machine learning by 2 methods: Separated and combined.
