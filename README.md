# frt-project
# ATLIQ-HARDWARE-SALES-INSHITE-DATA-VISULIZATION-
Microsoft Power Bi, Mysql, Data Wrangling.

//project is done using datavanalytics

Mysql database has all sales transactions, customers, products and markets information. I have analyse this database and than hook it up with power BI. In power BI I perform ETL and data cleaning operations to make it ready so that we can build our dashboard. Then build a powerful dashboard that can help us generate sales insights on Atliq hardware business. .


MYSQL QUEARY

## Sales Insights Data Analysis Project

### Data Analysis Using SQL

1. Show all customer records

    `SELECT * FROM customers;`

1. Show total number of customers

    `SELECT count(*) FROM customers;`

1. Show transactions for Chennai market (market code for chennai is Mark001

    `SELECT * FROM transactions where market_code='Mark001';`

1. Show distrinct product codes that were sold in chennai

    `SELECT distinct product_code FROM transactions where market_code='Mark001';`

1. Show transactions where currency is US dollars

    `SELECT * from transactions where currency="USD"`

1. Show transactions in 2020 join by date table

    `SELECT transactions., date. FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020;`

1. Show total revenue in year 2020,

    `SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.currency="INR\r" or transact
