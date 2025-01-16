# BankSphere-NoSQL-Customer-Behavior-Analysis

## Project Overview
This project focuses on the analysis of bank transactions and customer segmentation using a dataset sourced from Kaggle. The goal is to extract deeper insights into customer behaviors and identify factors contributing to account closures. By leveraging MongoDB's flexibility and aggregation capabilities, we aim to achieve meaningful conclusions about customer financial health and status. The analysis is conducted using Jupyter Notebook, which facilitates interactive and detailed data exploration.

## Dataset
- **Source**: [Credit Card Customers Prediction Dataset](https://www.kaggle.com/datasets/whenamancodes/credit-card-customers-prediction)
- **Description**: The dataset contains details about customer demographics, account attributes, and transactional data.

## Objectives
1. **Customer Segmentation**:
   - Classify customers based on age, gender, education level, and income category.
2. **Customer Status Analysis**:
   - Identify patterns and causes of account closures by analyzing the attrition flag and inactivity trends.
3. **Financial Health Assessment**:
   - Assess customers' financial health using metrics such as credit limit, revolving balance, and credit utilization ratios.

## Tools and Technologies
- **Jupyter Notebook(Lab)**: Used for interactive data exploration, analysis, and visualization.
- **MongoDB**: A NoSQL database for managing and storing structured and semi-structured data efficiently.

## MongoDB Collection Structure
### 1. Collection: `customers`
- **Fields**:
  - `CLIENTNUM`: Unique identifier for each customer
  - `Attrition_Flag`: Indicator of account closure
  - `Customer_Age`: Age of the customer
  - `Gender`: Gender of the customer
  - `Education_Level`: Education level of the customer
  - `Marital_Status`: Marital status of the customer
  - `Income_Category`: Income category of the customer
  - `Card_Category`: Type of card held by the customer

### 2. Collection: `transactions`
- **Fields**:
  - `CLIENTNUM`: Unique identifier linking to the customer
  - `Total_Trans_Amt`: Total transaction amount
  - `Total_Trans_Ct`: Total transaction count
  - `Total_Amt_Chng_Q4_Q1`: Change in transaction amount from Q4 to Q1
  - `Total_Ct_Chng_Q4_Q1`: Change in transaction count from Q4 to Q1
  - `Avg_Utilization_Ratio`: Average utilization ratio
  - `Credit_Limit`: Credit limit of the account
  - `Total_Revolving_Bal`: Total revolving balance

## Aggregation Ideas
### 1. Customer Segmentation
- Classification of customers based on:
  - Age
  - Gender
  - Education level
  - Income category

### 2. Customer Status Analysis
- Analyze causes of account closures by:
  - Evaluating the attrition flag
  - Monitoring inactivity trends over months

### 3. Financial Health Assessment
- Assess customers' financial health through:
  - Credit limit analysis
  - Revolving balance trends
  - Utilization ratio evaluation

## How to Run
1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   ```
2. **Install Dependencies**:
   Ensure you have the required Python libraries installed:
   ```bash
   pip install -r requirements.txt
   ```
3. **Set Up MongoDB**:
   - Import the dataset into MongoDB collections (`customers` and `transactions`).
4. **Run the Jupyter Notebook**:
   - Open JupyterLab and navigate to the notebook.
   - Execute the cells to perform data analysis.
