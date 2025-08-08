# Internal Controls Dashboard – Power BI Project



This Power BI project analyses a set of expense claims to assess compliance with internal controls, focusing on high-value claims and claims rejected due to missing approvals.

## 📊 Project Overview

The dashboard was created to help identify potential control breaches in an organisation's expense claim process. It focuses on two key areas:
- Claims that were **rejected** due to missing approvals
- Claims with an **amount over AUD $500**

## 🗂️ Data Sources

- **Expense Claim Dataset**: [Excelx - Finance & Accounting Practice Data](https://excelx.com/practice-data/finance-accounting/)
- **Exchange Rates**: Daily historical rates from the [Reserve Bank of Australia (RBA)](https://www.rba.gov.au/statistics/historical-data.html)

## 🔧 Data Preparation Steps

1. Imported both datasets into Power BI.
2. Created a relationship between the `ExpenseClaims` and `ExchangeRates` tables using a combined index of `Date + Currency`.
3. Converted all claim amounts into **AUD** using the appropriate historical exchange rate.
4. Created a new column to **flag claims over AUD $500**.
5. Built **two dashboards**:
   - **Rejected Claims Dashboard**
   - **High Amount Claims Dashboard**

## 📈 Dashboard Features

Each dashboard includes the following insights:
- Total number and value (in AUD) of claims by category
- Number of claims approved or rejected by managers
- Number of claims submitted by each employee
- Number of claims and amount of claims over time

## 🧠 Skills Demonstrated

- Data transformation using Power Query (M language)
- DAX calculations for flagging and categorisation
- Power BI relationships and data modelling
- Dashboard design and visualisation best practices
