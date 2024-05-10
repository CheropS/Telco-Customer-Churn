# Telco Customer Data Analysis 

## Introduction 
The dataframe is for Telco Customer Churn which has information on the details of the customers they have and how many are retained in the company. 
There are various variables including gender, contract type, payment details and type of customers. The aim of this analysis is to try and understand the data and see the relationship between gender, phone service, contract type and churn. 
The analysis will include conducting a linear and logistic regression to see the relationship between the x (gender, phone service, contract) and y(churn) variables.

## Steps

### Importing
We import the necessary for data processing, visualization, encoding, prediction libraries and one for ignoring warnings. 

### Loading the dataset
Get data from"https://www.kaggle.com/datasets/blastchar/telco-customer-churn" and downloaded to the local machine. 
When using local machine, add the file to your working folder (TELCO)
On your Google Drive, mount the downloaded data if you are using Google Colab 
When using local machine, add the file to your working folder (TELCO)
Disclaimer: If you have cloned the data, ignore the above steps

### Exploring the dataset
I explored the dataframe by checking the first and last ten rows. 
used the decribe function to see the mean, standard devation and percentile of the numerical data

df.info() to observe the data

### Data Cleaning 
Data cleaning involves preparing and processing telecommunications-related data to ensure its quality, accuracy, and consistency for analysis or modeling purposes. 
        - Check empty columns using df.isnull().sum()
        - fill empty cells using mean and median 
        - check for outliers which gave us TotalCharges because the data was a multiplication of monthy charges and tenure. Monthly charges then became an outlier. 


