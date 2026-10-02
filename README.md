# DATA_PROFILER_PR1
# Customer Churn Data Profiling Project

## 📌 Project Overview

This project focuses on Customer Churn Data Profiling and Analysis using a customer dataset collected from multiple data sources.

The project demonstrates how to:

- Import and inspect customer data
- Check data types, missing values, and duplicate records
- Clean and prepare the dataset
- Work with CSV, JSON, SQL, and API data sources
- Perform basic Exploratory Data Analysis (EDA)
- Analyze customer churn patterns
- Convert and work with structured JSON data
- Connect to SQL and fetch customer records
- Fetch customer data through an API
- Use Python and Pandas for data profiling

---

## 🎯 Objectives

The main objectives of this project are:

1. Understand the structure of the customer churn dataset.
2. Identify missing values and duplicate records.
3. Check and handle data types.
4. Clean and prepare the dataset.
5. Import data from different sources.
6. Convert and work with CSV and JSON data.
7. Fetch records from a SQL database.
8. Fetch customer data using an API.
9. Perform basic exploratory data analysis.
10. Identify patterns related to customer churn.

---

## 📊 Dataset Information

The dataset contains 31 records and 13 columns.

Columns included in the dataset:

- Customer_ID – Unique customer identifier
- Age – Customer age
- Gender – Customer gender
- City – Customer city
- Purchase_Frequency – Frequency of customer purchases
- Total_Purchases – Total number of purchases
- Average_Order_Value – Average value of customer orders
- Days_Since_Last_Purchase – Days since the last purchase
- Support_Tickets – Number of support tickets
- Discount_Used – Whether the customer used a discount
- Payment_Method – Customer payment method
- Churn – Customer churn status (Yes/No)
- Source – Original source of the data

---

## 🔍 Data Quality Check

The dataset was checked for common data-quality issues.

- Total Rows: 31
- Total Columns: 13
- Missing Values: 3
- Duplicate Rows: 1

Missing values are present in some fields such as:

- Support_Tickets
- Average_Order_Value
- Discount_Used

These missing values can be handled during the data-cleaning process.

---

## 🧹 Data Cleaning

The following data-cleaning operations are performed:

- Checking missing values
- Handling missing values
- Checking duplicate records
- Checking column data types
- Removing unnecessary data where required
- Standardizing data
- Preparing data for analysis

---

## 📥 Data Sources

This project demonstrates working with multiple data sources.

### 1. CSV

The original customer dataset is stored in CSV format.

File:

customer_churn_dataset_dataprofile_pr1(3).csv


### 2. JSON

The customer dataset is also available in JSON format.

File:

customer_churn_dataset_dataprofile_pr1(2).json


The JSON file stores each customer as an individual JSON object.

### 3. SQL

The project contains SQL commands for storing and retrieving customer churn records.

File:

customer_churn_dataset_dataprofile_pr1(1).sql


### 4. API

The project also demonstrates fetching customer data from a REST API and integrating the returned data with the dataset.

---

## 🐍 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- MySQL
- SQL
- REST API
- CSV
- JSON
- Jupyter Notebook
- Google Colab

---

## 📁 Project Structure

Customer-Churn-Data-Profiling/

│
├── customer_churn_dataset_dataprofile_pr1(3).csv
├── customer_churn_dataset_dataprofile_pr1(2).json
├── customer_churn_dataset_dataprofile_pr1(1).sql
├── data_profiler_Pr_1.ipynb
└── README.md

---

## ▶️ How to Run the Project

### Step 1: Install Required Libraries

Use the following command:

pip install pandas numpy matplotlib seaborn


### Step 2: Open the Notebook

Open:

data_profiler_Pr_1.ipynb

You can use:

- Google Colab
- Jupyter Notebook
- VS Code

### Step 3: Load the CSV File

Example:

import pandas as pd

df = pd.read_csv("customer_churn_dataset_dataprofile_pr1(3).csv")

print(df.head())
print(df.shape)
print(df.info())

### Step 4: Check Missing Values

print(df.isnull().sum())

### Step 5: Check Duplicate Records

print(df.duplicated().sum())

### Step 6: Basic Statistical Analysis

print(df.describe())

---

## 📈 Exploratory Data Analysis

The dataset can be analyzed using different customer-related variables such as:

- Age
- Purchase Frequency
- Total Purchases
- Average Order Value
- Days Since Last Purchase
- Support Tickets
- Discount Used
- Payment Method
- Churn

Example:

import matplotlib.pyplot as plt
import seaborn as sns

sns.countplot(data=df, x="Churn")
plt.title("Customer Churn Distribution")
plt.show()

---

## 🔗 SQL Data Fetching

The SQL database can be created using:

CREATE DATABASE customer_churn;

USE customer_churn;

SELECT *
FROM customer_churn;

The database and table names should match the SQL file used in the project.

---

## 🌐 API Data Fetching

Customer data can be fetched from a REST API using Python.

Example:

import requests

response = requests.get("YOUR_API_URL")

if response.status_code == 200:
    data = response.json()
    print(data)
else:
    print("API request failed")

The API data can then be converted into a Pandas DataFrame for further analysis.

---

## 📄 JSON Data Example

A customer record is stored in JSON format like this:

{
  "Customer_ID": 1001,
  "Age": 24,
  "Gender": "Male",
  "City": "Surat",
  "Purchase_Frequency": "Monthly",
  "Total_Purchases": 3,
  "Average_Order_Value": 1850.0,
  "Days_Since_Last_Purchase": 12,
  "Support_Tickets": 1.0,
  "Discount_Used": "No",
  "Payment_Method": "UPI",
  "Churn": "No",
  "Source": "CSV"
}

---

## 💡 Key Learning Outcomes

Through this project, the following concepts are demonstrated:

- Data collection
- CSV file handling
- JSON parsing
- SQL database connectivity
- API data fetching
- Data cleaning
- Missing-value handling
- Duplicate detection
- Data-type checking
- Exploratory Data Analysis
- Data visualization
- Customer churn analysis

---

## 🚀 Future Improvements

This project can be further improved by adding:

- Customer churn prediction
- Logistic Regression
- Decision Tree
- Random Forest
- Confusion Matrix
- Model Accuracy
- Customer Segmentation
- Interactive Dashboard
- Automated API Data Collection
- Advanced Statistical Analysis

---

## 📝 Conclusion

The Customer Churn Data Profiling project demonstrates how customer data can be collected, cleaned, analyzed, and managed using multiple data sources.

The project combines CSV, JSON, SQL, and API data with Python-based data analysis.

It provides a foundation for further development into a complete Customer Churn Prediction and Machine Learning project.

---

## ⭐ Project Status

Completed – Data Profiling and Multi-Source Data Handling


AUTHOR 
PATHAN SAHIL
