# Olist-Business-Analysis
This is a project to analyse on the customers, products and orders of the Brazilian E-commerce giant Olist.

### Brief
TODO:

### Objective
TODO:

## Table of Contents
- [Prerequisite to use](#prerequisite-to-use)
  - [Libraries](#libraries)
  - [SQL authorisation](#sql-authorisation)
- [Database Schema](#database-schema)
- [Analysis Results](#analysis-results)
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

# Database Schema
The scraped data will be cleaned, transformed, loaded and stored in Azure SQL Database:

![image](https://github.com/NoahPlage/Olist-Business-Analysis/blob/main/img/database-schema.png)

# Power BI Dashboard
You can find the Dashboard, the project file and the converted version to PDF below:

![image](https://github.com/NoahPlage/Olist-Business-Analysis/blob/main/img/powerbi-p1.png)

![image](https://github.com/NoahPlage/Olist-Business-Analysis/blob/main/img/powerbi-p2.png)


| Format | Link |
|--|--|
|Power BI online|[Link](https://app.powerbi.com/view?r=eyJrIjoiMTc0YmQyN2QtMmY4ZS00ZDhjLWE1YmUtMzE3MTczNWQ3YThiIiwidCI6IjI1YTk5YmYwLThlNzItNDcyYS1hZTUwLWFkZmJkZjBkZjZmMSIsImMiOjEwfQ%3D%3D&pageName=ReportSection)|
|Power BI offline|[.pbix](https://github.com/NoahPlage/Olist-Business-Analysis/blob/main/docs/olist-business-analysis.pbix)|
|PDF|[.pdf](https://github.com/NoahPlage/Olist-Business-Analysis/blob/main/docs/olist-business-analysis.pdf)|

# Contributers
Hello World!

- [Angela](https://www.linkedin.com/in/angela-p-171b30136/)
- [Brandon](https://www.linkedin.com/in/jinheng-lim/)
- [Mavis](https://www.linkedin.com/in/mavis-luo-3a5b76192/)
- [Soon Chye](https://www.linkedin.com/in/lim-soonchye/)
