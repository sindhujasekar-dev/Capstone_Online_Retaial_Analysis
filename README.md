### Customer Retention: Churn Prediction, Segmentation Analysis

**Sindhuja Sekar**

#### Executive summary
This project analyzes customer transaction data from an online retail business to understand purchasing behavior, identify churn patterns, and generate business insights for customer retention. The analysis includes exploratory data analysis (EDA), data preprocessing, feature engineering, customer churn prediction, and customer segmentation techniques.

Customer-level behavioral features such as Recency, Frequency, and Monetary value (RFM) were derived from transaction data to study customer engagement patterns. Machine learning models were used to establish a baseline churn prediction framework, while clustering techniques helped identify distinct customer segments. The findings provide insights into customer retention behavior and support data-driven business decision-making.

#### Rationale
Why should anyone care about this question?
Customer retention is one of the most important challenges in e-commerce businesses. Acquiring new customers is often more expensive than retaining existing ones. Understanding why customers stop purchasing and identifying patterns in customer behavior can help businesses improve retention strategies, optimize marketing efforts, and increase long-term revenue.

Identify customer purchasing patterns associated with churn risk and customer retention.

#### Research Question
What are you trying to answer?
Can customer transaction patterns help predict churn risk?
Which customer groups are more likely to remain active or churn?
How can customer segmentation support retention strategies?

#### Data Sources
What data will you use to answer you question?
Dataset used:

Online Retail Dataset from the UCI Machine Learning Repository
UCI Online Retail Dataset - https://archive.ics.uci.edu/dataset/352/online+retail

Dataset characteristics:
Contains online retail transactions from a UK-based e-commerce business
Includes customer purchases between 2010 and 2011
Contains transaction details such as:
Invoice number
Product description
Quantity purchased
Unit price
Invoice date
Customer ID
Country

#### Methodology
What methods are you using to answer the question?
1. Data Cleaning and Preprocessing
Removed invalid transactions with negative quantities and prices
Handled missing CustomerID values
Converted date columns into datetime format
Created revenue-related features

2. Exploratory Data Analysis (EDA)

EDA was performed to analyze:
Sales and revenue trends
Customer purchasing patterns
Country-wise transaction behavior
Product-level sales distribution
Customer activity behavior

Visualizations were created using Matplotlib and Seaborn.

3. Feature Engineering
Customer-level features were generated using RFM concepts:
Recency
Frequency
Monetary Value

These features were used for churn analysis and machine learning modeling.

4. Churn Definition
Since the dataset did not contain a churn label, churn was defined based on customer inactivity:
Customers with no purchases within the last 90 days were labeled as churned customers.


#### Results
What did your research find?
Key Findings
Customers with higher purchase frequency were less likely to churn.
Customers purchasing in larger quantities generally showed stronger retention behavior.
Geographic patterns indicated relatively higher churn tendencies among some non-UK customers.
Monetary spending alone was not the strongest indicator of retention behavior.
Recency and Frequency contributed significantly to churn prediction performance.
Model Insights
Supervised Machine learning algorithm - Logistic Regression established a baseline churn prediction model.

#### Next steps
What suggestions do you have for next steps?
Using unsupervised algorithm K-Means clustering was applied to group customers based on purchasing behavior and engagement patterns.
Using Random Forest to improve predictive performance and feature importance insights.
Customer segmentation will groups customer as:
loyal customers
high-value customers
at-risk customers
low-engagement customers

Based on the results will apply business insights to retain customers.

#### Outline of project
Phase - 1: https://github.com/sindhujasekar-dev/Capstone_Online_Retaial_Analysis/blob/main/Phase_1_Online_retail_EDA.ipynb
