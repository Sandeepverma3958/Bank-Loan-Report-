# 🏦 Bank Loan Analytics Dashboard — Power BI

## 📌 Project Overview

The **Bank Loan Analytics Dashboard** is an end-to-end Business Intelligence project built using **SQL Server and Power BI** to analyze a bank's loan portfolio from application and funding to repayment.

The project transforms raw loan data into an interactive three-page Power BI report that helps management understand **loan demand, lending performance, repayment, customer characteristics, regional distribution, and portfolio quality**.

The main objective is not only to visualize loan data, but to answer important business questions and help management identify **growth opportunities, portfolio trends, and potential credit-risk areas**.

---

# 🎯 Business Problem

Banks generate a large amount of loan-related data, including applications, funded amounts, interest rates, customer information, repayment amounts, loan grades, and loan status.

Without proper analysis, it can be difficult for management to understand:

* How loan applications are changing over time
* How much money is being funded
* How much money is being recovered
* Whether the loan portfolio is improving or deteriorating
* What percentage of loans are performing versus bad
* Which regions generate the highest loan demand
* What types of customers are taking loans
* Which loan purposes and credit grades are associated with the portfolio
* Where potential credit-risk concentrations exist

This project addresses these problems by creating an interactive Power BI reporting solution that converts raw loan data into **actionable business insights**.

---

# ❓ Business Questions Answered

The dashboard is designed to answer questions such as:

### Loan Performance

* How many loan applications has the bank received?
* How is the number of applications changing month-over-month?
* What is the Month-to-Date (MTD) loan application performance?
* How much has the bank funded?
* How much money has been received from borrowers?
* How are funded and received amounts changing over time?

### Portfolio & Risk

* What percentage of loans are classified as Good Loans?
* What percentage are classified as Bad Loans?
* How much has been funded to Good Loans versus Bad Loans?
* How much has been received from Good Loans versus Bad Loans?
* What is the average interest rate?
* What is the average Debt-to-Income (DTI) ratio?
* How are these KPIs changing compared with the previous month?

### Regional & Customer Analysis

* Which regions generate the highest number of loan applications?
* Which regions receive the highest amount of funding?
* What loan terms are most commonly selected?
* How are loans distributed according to homeownership?
* What types of customers contribute most to the loan portfolio?

### Loan-Level Analysis

* What is the purpose of individual loans?
* What are the customer's Grade and Sub Grade?
* When was the loan issued?
* How much was funded?
* What interest rate was applied?
* What is the installment amount?
* How much has been received against the loan?

---

# 📊 Dashboard Structure

The report consists of **three interactive dashboards**.

## 1. Summary Dashboard

The Summary page provides a high-level view of the overall loan portfolio.

### Key KPIs

* Total Loan Applications
* MTD Loan Applications
* MoM Loan Applications
* Total Funded Amount
* MTD Funded Amount
* MoM Funded Amount
* Total Amount Received
* MTD Amount Received
* MoM Amount Received
* Average Interest Rate
* MTD Average Interest Rate
* MoM Average Interest Rate
* Average DTI
* MTD Average DTI
* MoM Average DTI

It also provides a **Good Loan vs Bad Loan** analysis.

For this project, loans are classified as:

**Good Loans**

* Current
* Fully Paid

**Bad Loans**

* Charged Off

The dashboard compares Good and Bad Loans based on:

* Loan Applications
* Funded Amount
* Amount Received
* Percentage of total loans

This helps management understand both **loan performance and portfolio quality**.

---

## 2. Overview Dashboard

The Overview page focuses on **regional, customer and loan characteristics**.

It provides:

* Loan Applications by Region
* Loan Distribution by Term
* Loan Distribution by Homeownership
* Additional portfolio analysis by customer/loan characteristics

The regional map helps identify areas with higher loan demand and lending concentration.

The loan-term analysis shows customer preference for different repayment periods.

The homeownership analysis provides insight into the customer profile and allows the portfolio to be examined across different housing categories.

These analyses can help management identify **market opportunities and potential areas of risk concentration**.

---

## 3. Details Dashboard

The Details page provides a **loan-level view** of the portfolio.

The report contains information such as:

* Loan ID
* Purpose
* Home Ownership
* Grade
* Sub Grade
* Issue Date
* Funded Amount
* Interest Rate
* Installment
* Amount Received

This page allows users to move from high-level portfolio analysis to individual loan records and investigate the underlying data.

For example, if a particular region or loan grade shows unusual performance, users can use the Details page to investigate the underlying loans.

---

# 🛠️ Technology Stack

## SQL Server

SQL Server was used as the primary data source and for data validation and analysis.

The dataset was connected directly from the SQL Server database to Power BI.

SQL was also used to independently verify important calculations and KPIs generated in Power BI.

### SQL Concepts Used

* Creating Database
* Creating Tables
* SELECT
* DISTINCT
* COUNT
* GROUP BY
* ORDER BY
* CTE (Common Table Expressions)
* PARTITION BY
* DATENAME
* DATEPART
* MONTH
* DAY
* HOUR
* QUARTER
* CAST
* DECIMAL
* LIMIT

SQL queries created for **cross-verification and validation** are included in this repository.

This helped ensure that the numbers displayed in the Power BI dashboard were consistent with the underlying database calculations.

---

# 📈 Power BI

Power BI was used to transform the SQL data into an interactive Business Intelligence solution.

### Power BI Concepts Used

* Connecting to SQL Server
* Data Cleaning
* Data Processing
* Power Query
* Data Modelling
* Relationships
* Date Tables
* Time Intelligence
* DAX
* Date Functions
* Text Functions
* Filter Functions
* CALCULATE
* SUM
* SUMX
* KPI Creation
* Card Visuals
* Charts
* Visual Formatting
* Navigation
* Interactive Dashboard Design
* Report Page Navigation

---

# 🔄 Project Workflow

The project follows an end-to-end BI workflow:

**SQL Server Database**

⬇️

**Data Extraction**

⬇️

**Power BI Connection**

⬇️

**Data Cleaning & Processing**

⬇️

**Data Modelling**

⬇️

**Date Table Creation**

⬇️

**DAX Measures & Calculations**

⬇️

**KPI Development**

⬇️

**Interactive Visualizations**

⬇️

**Business Analysis**

⬇️

**SQL Cross-Verification**

---

# 🔍 Data Validation & Cross-Verification

An important part of the project was validating the Power BI results independently.

After creating KPIs and calculations in Power BI, I created SQL queries to calculate the corresponding metrics directly from the database.

The SQL results were then compared with the Power BI results to verify the accuracy of the analysis.

The SQL verification queries are included in this repository.

This approach helped ensure that the dashboard was not only visually interactive but also **data-driven and reliable**.

---

# 💡 Business Value

The dashboard can help bank management:

* Monitor loan demand and lending performance
* Track funding and repayment trends
* Compare current performance with previous months
* Monitor Good Loan and Bad Loan proportions
* Identify regions with high loan demand
* Understand customer and loan characteristics
* Investigate loan-level performance
* Identify potential portfolio-risk concentrations
* Support data-driven lending and portfolio-management decisions

---

# 🎓 Key Learning Outcomes

This project provided practical experience in building an **end-to-end Business Intelligence solution**.

The major learning outcomes include:

* Working with data stored in SQL Server
* Writing SQL queries for business analysis
* Validating BI calculations using SQL
* Connecting Power BI with SQL Server
* Cleaning and processing data using Power Query
* Building a structured data model
* Creating and using Date Tables
* Applying DAX for business calculations
* Implementing time-intelligence analysis
* Creating KPIs and interactive visuals
* Designing dashboard navigation
* Translating business requirements into analytical solutions
* Presenting data in a business-friendly storytelling format

---

# 📁 Repository Structure

```text
Bank-Loan-PowerBI-Project/
│
├── PowerBI/
│   └── Bank_Loan_Report.pbix
│
├── SQL/
│   └── SQL_Queries_and_Cross_Verification.sql
│
├── Dataset/
│   └── Bank_Loan_Data
│
├── Screenshots/
│   ├── Summary.png
│   ├── Overview.png
│   └── Details.png
│
└── README.md
```

---

# 🚀 Project Outcome

The final solution transforms raw bank loan data into a **three-level analytical reporting system**:

**Summary → What is happening?**

**Overview → Where and among whom is it happening?**

**Details → Which individual loans are driving the result?**

This structure enables users to move from **high-level business performance to deeper analysis and individual loan investigation**, making the report useful for both management-level monitoring and detailed portfolio analysis.
