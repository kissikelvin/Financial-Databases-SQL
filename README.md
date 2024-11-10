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

The project is organized into several main sections:

Data Population in SQL Database

We start by preparing the dataset. This includes defining the tickers that compose the Fintech ETF and populating a SQL database with market data using the Yahoo Finance API. Then, we add daily returns to this database. The functions for these tasks are stored in utils.py.

Single Asset Analysis in the ETF

This section focuses on analyzing an individual stock within the ETF. Here, we calculate daily returns, visualize the stock's performance, and evaluate its contribution to the overall ETF.

Enhanced Data Access with Advanced SQL Queries

In this part, we optimize data retrieval by writing advanced SQL queries. This improves data access efficiency, which is critical for handling large datasets effectively.

ETF Portfolio Analysis

We analyze the ETF as a combined portfolio by aggregating data from all four stocks. This includes calculating overall daily returns and generating insights into the ETF's overall performance.

Creating a New Database for Equal-Weighted ETF Returns

To maintain the integrity of the original data, we create a new database to store daily returns for an equally weighted ETF. This approach preserves the original etf.db database for additional analysis.

Notebook Deployment as a Web Application

Finally, we deploy the Jupyter Notebook as a web application using the Voilà library. This enables users to explore ETF data and visualizations interactively through a browser interface.
