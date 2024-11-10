# DB_WebApp_using_SQL

*by KELVIN KISSI*

![Display](Resources/DBsql.png)

---

## Background

# Table of Contents

1. [Installation](#installation)
2. [Basic Usage](#basic-usage)
    1. [Quick Start](#quick-start)
    3. [Collecting information from the database](#collecting-information-from-the-database)
    3. [Searching the database extensively](#searching-the-database-extensively)
    4. [Storing the database at a different location](#storing-the-database-at-a-different-location)
6. [Contact](#contact)


# Project Outline

The project is structured into several key parts:

Populating Data into SQL Database

We begin by preparing the data. First, we define the tickers that make up the Fintech ETF and populate a SQL database with the relevant market data using the Yahoo Finance API. Next, we add the daily returns to the created SQL database. The functions to perform these tasks are stored in utils.py.
Analyze a Single Asset in the ETF

In this section, we perform individual analysis on a selected stock in the ETF. This includes calculating daily returns, visualizing the stock's performance, and understanding its contribution to the overall ETF.
Optimize Data Access with Advanced SQL Queries

Here, we focus on improving the efficiency of data access. By writing additional SQL queries, we can retrieve and process stock data more efficiently, which is crucial for optimizing performance, especially when handling large datasets.
Analyze the ETF Portfolio

This part involves analyzing the ETF as a whole, combining the data of all four stocks. We compute the overall daily returns and provide insights into the performance of the ETF as a portfolio.
Create a New Database for Equal-Weighted ETF Returns

In order to preserve the original data, we create a new database to store the daily returns of the ETF, assuming the stocks are equally weighted. This ensures that the original etf.db database remains unaltered while we perform further analysis.
Deploy the Notebook as a Web Application

Finally, we use the Voilà library to deploy the Jupyter Notebook as a web application. This step allows users to interact with the analysis through a browser-based interface, enabling real-time exploration of the ETF data and visualizations.
