# Customer Performance Report Using PowerBI

![PowerBI Dashboard](image-housing.jpg)

## Project Overview
This project leverages PowerBI to analyze and visualize customer performance data from a retail company. It aims to provide insights into demographics, purchase behaviors, and revenue patterns to aid strategic decision-making and enhance marketing efforts.

## Data Description
The dataset includes six CSV files:
- **Customer**: Data on each customer, including age, whether they have children, etc.
- **Geography**: Geographic data related to customers.
- **Product**: Information on products such as ID, category, and price.
- **Date**: Date dimensions for temporal analysis.
- **Sales Territory**: Details about sales territories.
- **Fact Internet**: Sales transaction records.

These files are integrated within PowerBI to create a comprehensive data model for multi-dimensional analysis of sales performance.

## Data Source
The dataset is provided in CSV format.  
[Download Raw Dataset Here](NashvilleHousing.csv)

## Tools Used
- **Microsoft Power BI**: Employed for data cleaning, transformation, exploration, and visualization.

## Key Insights
This Customer Performance Report generates several key insights:
- **Total Revenue**: Summarizes total sales revenue.
- **Average Age of Customers**: Calculates the average age across all customers.
- **Total Count of Customers**: Enumerates total number of customers within the dataset.
- **Customer Categorization**: Classifies customers based on their order history and purchasing volumes:
  - **VIP Customers**: Customers with at least 2 orders and total purchases of $100 or more.
  - **Loyal Customers**: Customers who have placed multiple orders regardless of purchase value.
  - **Periodic Buyers**: Customers with fewer interactions and smaller purchase volumes.
- **Revenue Analysis by Parental Status**: Analyzes differences in revenue between customers who have children and those who do not.
- **Dynamic Ranking System**: Implements a system to rank top-performing customers based on frequency, monetary value, and recent purchases.
- **Revenue Based on Gender**: Examines revenue generation segmented by customer gender.

## PowerBI Techniques Used

### Variables
- **Customer Age**: Indicates the age of the customer.
- **CustomerWithChildren**: Indicates whether customers have children.
- **Age Category**: Categorizes customers into age brackets.
- **Top Country**: Identifies the country with the highest number of customers without children.

### Measures
- **Total Revenue**: Captures the total sales revenue.
- **Customer Count**: Counts the number of unique customers.
- **Total Revenue From Customers with Children**: Aggregates revenue from customers who have children.
- **Total Revenue From Customers without Children**: Aggregates revenue from customers without children.
- **Average Revenue By Age Group**: Computes the average revenue per age category.

### Visualization Techniques
- **Conditional Formatting**: Enhances readability and visual appeal of reports.
- **Interactive Filters**: Allows users to customize data views according to various parameters.
- **Dynamic Ranking**: Features tables that update dynamically to showcase top-performing customers.

## SQL Code for Data Preparation
For the rest of the code, check the [SQL Code](nashville-housing.sql) file.
```sql
CREATE DATABASE nashville_housing;
---import nashville housing csv file

SELECT *
FROM nashville_housing.dbo.nashville;


