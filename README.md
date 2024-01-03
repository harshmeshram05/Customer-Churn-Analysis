# Customer-Churn-Analysis

## Project Overview
This project offers an in-depth analysis of bank churn data. Churn in this context signifies the number of customers who have left the bank, commonly referred to as attrition. The dataset used for this analysis is a sample, utilized for the purpose of practicing report creation and understanding the various aspects of data analysis using PowerBI.

## Objective
- Understand and analyze the factors contributing to customer churn.
- Develop actionable insights from the data to help reduce churn.

## Workflow

### 1. Data Connection
Establish a stable connection to the source of the bank churn data.

### 2. Data Preparation
Data cleaning and preparation are crucial for accurate analysis. The following steps outline the data preparation process:

- Check data types and column names.
- Remove the 'Estimated Salary' column.
- Ensure column names begin with a capital letter.
- Rename columns to:
  - Credit Scores
  - Credit Card Status
  - Active Status
  - Churn Status
- Add an example column for products (e.g., Product 1).
- Modify values for clarity and understanding:
  - Churn Status: 1 – Churned, 0 – Not Churned
  - Active Status: 1 – Active, 0 – Inactive
  - Credit Card Status: 1 – Owned, 0 – Not Owned
- Introduce conditional columns based on existing data:
  - Age Groups (derived from Age)
  - Credit Scores (derived from Credit Score)
  - Account Balance (derived from Balance)

### 3. Data Modeling and Analysis
Construct reference tables and develop conditional columns:

- Create a reference table from the customer data table, rename it to 'Age Groups', retain only the 'Age Groups' column, and eliminate duplicates.
- Introduce an 'Age Group ID' conditional column in the 'Age Groups' table.
- Similarly, create reference tables for 'Account Balance' and 'Credit Scores'. Insert respective IDs as conditional columns.

### 4. Creating Measures
Develop measures to further aid the analysis:

- Measure to calculate the number of customers.
- Measure to calculate the number of lost customers.
- Measure to calculate the churn rate.

### 5. Data Visualization
Visual representation of data offers intuitive insights. The following visuals will be incorporated in the report:

**Cards**:
- Displaying the number of customers.
- Displaying the churn rate.

**Slicer**:
- Churn Status

**Charts**:
- Donut charts for:
  - Number of customers by gender.
  - Number of customers by activity status.
  - Number of customers by credit card status.
  - Number of customers by country.
  - Number of customers by products.
- Line and clustered column chart showing customers and churn rate by age group.
- Line and clustered column chart showing customers and churn rate by credit score.
- Line and clustered column chart showing customers and churn rate by account balance

