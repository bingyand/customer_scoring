# customer_scoring

## Table of contents
* [General info](#general-info)
* [Prerequisites](#prerequisites)
* [Datasets](#datasets)

## General info
This project is created to evaluate each active customer's value and the risk of conducting rejected/failed transactions. Customer value are determined based on three criteria: Recency, Frequency, and Monetary Value. 

- Recency: How recently a customer has made a purchase
- Frequency: How often a customer makes a purchase
- Monetary Value: How much money a customer spends on purchases

Each customer will be assigned a score from 1 to 4 for each critera, with 1 being the least valuable. Then, a total RFM_Score will be calcualted.

The customer rejected transaction risks are evaluated based on the number of rejected transactions, as well as the monetary value involved in rejected transactions. The following metrics are used into calculations:

- Total transaction amount
- Total transaction monetary value
- Rejected transaction amount
- Rejected transaction monetary value

On top of those metrics, the percentage of rejected trx amount versus total amount of trx, and the percentage of rejected trx monetary value versus total spending will be calculated. 

Combining the customer value and rejected transaction risk will help us to make the decision of customer relationship termination. 
	
## Prerequisites
To run this project, install the following required Python libraries:

- Numpy
- Pandas
- Date time
	
## Datasets
To run this project, download the follwing datasets:

Download all of the transaction data from 08-01-2019 to today. Since we are currenly experiencing the data retrival issue on the portal, please download all the datasets in the folder and concat accordingly. 
