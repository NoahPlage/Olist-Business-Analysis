# Olist-Business-Analysis
This is a project to analyse on the customers, products and orders of the Brazilian E-commerce giant Olist.

### Brief
Olist Store is the largest department store in Brazilian marketplaces. Olist connects small businesses from all over Brazil to channels without hassle and with a single contract. The Brazilian ecommerce public dataset of orders (from 2016 to 2018) made at Olist Store is provided to your company for analysis.

Your manager is asking you to critically analyse the provided datasets using Business Intelligence tools and provide some marketing findings / recommendations in a report format. The dataset has information of 100k orders made at multiple marketplaces in Brazil. Its features allow viewing an order from multiple dimensions: from order status, price, payment and freight performance to customer location, product attributes and finally reviews written by customers. A geolocation dataset that relates Brazilian zip codes to lat/lng coordinates is also integrated in the dataset.

After a customer purchases the product from Olist Store, a seller gets notified to fulfill that order. Once the customer receives the product, or the estimated delivery date is due, the customer gets a satisfaction survey by email where they can give a note for the purchase experience and write down some comments.

### Objective
1. Create data pipeline to ingest data in PostgreSQL or SQL server database
2. Use Power BI to answer following questions:
    - How many customers, orders, and orders per customer does the company have?
    - What is the number of customers by state?
    - What is the number of orders by month?
    - What are the top 5 product categories?
    - Visualise the company’s customers’ demographics, sales trend, orders by categories, orders changes by year, etc. and use Power BI to help make better decisions
3. Map and compare report data with data from database query to validate the reports
4. Critically analyse relevant data using statistical methods
5. Provide some recommendations and improvements

## Table of Contents
- [Prerequisite to use](#prerequisite-to-use)
  - [Libraries](#libraries)
  - [Required files](#required-files)
  - [SQL authorisation](#sql-authorisation)
- [Database Schema](#database-schema)
- [Power BI Dashboard](#power-bi-dashboard)
- [Contributers](#contributers)

## Prerequisite to use
### Libraries
Install the following libraries:

```
pandas
pyodbc
dotenv
seaborn
matplotlib
mpl_toolkits.basemap
re
nltk
sklearn
google_trans_new
```

### Required Files
Install Microsoft ODBC Driver for SQL Server (x64) from [here](https://docs.microsoft.com/en-us/sql/connect/odbc/download-odbc-driver-for-sql-server?view=sql-server-ver15#download-for-windows).

### SQL Authorisation
Azure SQL Database is used to store the datasets in this project.

You will need to insert your database connection parameters and save as `sql-keys.env` local file.

```
DB_SERVER = "XXXXX"
DB_NAME = "XXXXX" 
DB_USERNAME = "XXXXX"
DB_PASSWORD = XXXXX
```
The following is the list of the connection parameters:
- *DB_SERVER*: database server address e.g., localhost or an IP address.
- *DB_NAME*: the name of the database that you want to connect.
- *DB_USERNAME*: the username used to authenticate.
- *DB_PASSWORD*: password used to authenticate.

## Database Schema
The scraped data will be cleaned, transformed, loaded and stored in Azure SQL Database:

![image](https://github.com/NoahPlage/Olist-Business-Analysis/blob/main/img/database-schema.png)

## Power BI Dashboard
You can find the Dashboard, the project file and the converted version to PDF below:

![image](https://github.com/NoahPlage/Olist-Business-Analysis/blob/main/img/powerbi-p1.png)

![image](https://github.com/NoahPlage/Olist-Business-Analysis/blob/main/img/powerbi-p2.png)


| Format | Link |
|--|--|
|Power BI online|[Link](https://app.powerbi.com/view?r=eyJrIjoiMTc0YmQyN2QtMmY4ZS00ZDhjLWE1YmUtMzE3MTczNWQ3YThiIiwidCI6IjI1YTk5YmYwLThlNzItNDcyYS1hZTUwLWFkZmJkZjBkZjZmMSIsImMiOjEwfQ%3D%3D&pageName=ReportSection)|
|Power BI offline|[.pbix](https://github.com/NoahPlage/Olist-Business-Analysis/blob/main/docs/olist-business-analysis.pbix)|
|PDF|[.pdf](https://github.com/NoahPlage/Olist-Business-Analysis/blob/main/docs/olist-business-analysis.pdf)|

## Contributers
Hello World!

- [Angela](https://www.linkedin.com/in/angela-p-171b30136/)
- [Brandon](https://www.linkedin.com/in/jinheng-lim/)
- [Mavis](https://www.linkedin.com/in/mavis-luo-3a5b76192/)
- [Soon Chye](https://www.linkedin.com/in/lim-soonchye/)

<div align="right">
    <b><a href="#">↥ back to top</a></b>
</div>
