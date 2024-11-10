# DB_WebApp_using_SQL

*by KELVIN KISSI*

![Display](Resources/DBsql.png)

---

# Table of Contents

- [Installation](#installation)
   
This project is built in a Jupyter Notebook. If you don’t have Jupyter installed, you can follow the instructions [here](https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html) to set it up.

### Required Libraries

You can install all the necessary libraries by using the provided `requirements.txt` file. To install the dependencies, follow these steps:

1. **Download the `requirements.txt` file** included in the project repository.
2. Open a terminal and navigate to the project directory where the `requirements.txt` file is located.
3. Run the following command to install all the required packages:

   ```bash
   pip install -r requirements.txt
   ```

This will install the following libraries:
- **`numpy`**: For numerical computations.
- **`pandas`**: For data manipulation and DataFrame operations.
- **`hvplot`**: For creating interactive visualizations.
- **`sqlalchemy`**: For connecting and interacting with the SQL database.

### Manually Installing Specific Libraries (If Needed)

If you'd like to manually install any missing libraries, here are the installation commands:
- **SQLAlchemy**:
  ```bash
  pip install SQLAlchemy
  ```
- **Voilà** (optional for deploying as a web app):
  ```bash
  conda install -c conda-forge voila
  ```
Once the required packages are installed, you’ll be ready to run the project.
---

   
3. [Basic Usage](#basic-usage)
    1. [Quick Start](#quick-start)
    3. [Collecting information from the database](#collecting-information-from-the-database)
    3. [Searching the database extensively](#searching-the-database-extensively)
    4. [Storing the database at a different location](#storing-the-database-at-a-different-location)
6. [Contact](#contact)


# Background

In this project, we create a financial database and web application to analyze the performance of a hypothetical FinTech Exchange-Traded Fund (ETF). Built with SQL, Python, and the Voilà library, the application focuses on four stocks in the ETF: GDOT (Green Dot Corporation), GS (Goldman Sachs), PYPL (PayPal Holdings), and SQ (Block, formerly Square). Each stock has a dedicated table in the etf.db database, with data sourced from the Yahoo Finance API.

The analysis examines daily returns for each individual stock as well as the overall ETF performance. After completing the analysis, visualizations are deployed as a web application using the Voilà library, which transforms the Jupyter Notebook into an interactive web interface.


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
