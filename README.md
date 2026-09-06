# Customer Behavior Analysis — Shopping Trends
An end-to-end data analysis project that explores customer shopping behavior using Python for data cleaning, SQL for business-question analysis, and Power BI for interactive dashboard visualization.
# Project Overview
This project analyzes a retail shopping trends dataset to uncover customer purchasing patterns, revenue drivers, and behavioral segments. The workflow covers the complete data analytics pipeline:
1. Data Cleaning & Feature Engineering — Python (Pandas, NumPy)
2. Business Question Analysis — SQL (PostgreSQL)
3. Data Visualization — Power BI Dashboard

The goal was to simulate a real-world analytics workflow: taking a raw dataset, cleaning and enriching it, querying it to answer stakeholder-style business questions, and finally presenting insights through an interactive dashboard.

# Dataset
Source:[ Shopping Trends Dataset — Kaggle](https://www.kaggle.com/code/hasaankhan175/shopping-trends-eda-analysis)
Size: 3,900 rows × 18 columns
Description: Contains customer-level retail transaction data including demographics, purchase details, ratings, subscription status, discounts, and shipping preferences.

Column	                  Description
Customer ID	              Unique identifier for each customer
Age	                      Customer's age
Gender	                  Customer's gender
Item Purchased	          Product bought
Category	                Product category (Clothing, Footwear, etc.)
Purchase Amount (USD)	    Transaction value
Location	                Customer's location
Size, Color, Season	      Product attributes
Review Rating	            Rating given by customer
Subscription Status	      Whether customer is subscribed
Shipping Type	            Delivery method used
Discount Applied         	Discount usage flags
Previous Purchases      	Number of past purchases
Payment Method	          Mode of payment
Frequency of Purchases	  How often the customer shops


# Data Cleaning & Feature Engineering (Python)
Using NumPy and Pandas, the raw dataset was cleaned and enriched before analysis:
1. Loaded the dataset and inspected structure using .info() and .isnull().sum()
2. Identified missing values in the Review Rating column and imputed them using the median, to avoid distortion from outliers
3. Removed duplicate/redundant columns to keep the dataset clean and analysis-ready
4. Engineered new features to support deeper analysis:
  - age_group — bucketed customers into segments (e.g., Young Adult, Adult, Middle-aged, Senior) for demographic-level insights
  - purchase_frequency_days — converted the categorical purchase frequency (e.g., "Weekly", "Monthly") into a numeric day-based value for quantitative analysis
5. Exported the cleaned dataset for use in SQL analysis.

# customer-behavior-analysis/
    └── customer_behaviour.ipynb   


