# Telco-Churn-Customer-Analysis
# Description of Project
The dataset contains customer information from a telecommunications / subscription-based service company, that requires investigation of churn dynamics over a wide range of consumer profiles and behaviors. This study will help guide strategic decisions targeted at increasing customer satisfaction, retention, loyalty, and long-term profitability.

# Project Objective
To analyze the rate of customer churn across multiple categories. The project's goal is to identify insights into factors influencing customer retention and attrition by evaluating turnover rates across different categories. To provide actionable insights and recommendations for reducing churn, improving client retention methods, and optimizing company results.

# Data Cleaning
The dataset was loaded and explored using Power Query in Microsoft Excel. Upon initial inspection, it was observed that the dataset was generally well-structured, with appropriately named columns and no duplicate records or major errors. However, a few adjustments were made to enhance data consistency and prepare it for analysis.

Specifically, for the ‘Senior Citizen’ column, the data type was changed to Text, and the numeric values 0 and 1 were replaced with ‘No’ and ‘Yes’ respectively, to improve readability. In the ‘TotalCharges’ column, less than 1% of the cells were empty. A closer review revealed that these entries belonged to newly onboarded customers who had yet to make any payments. To ensure data completeness and avoid analytical issues, the null values were replaced with 0.

These minimal but important transformations helped maintain data integrity, consistency, and compatibility — all essential for accurate analysis and informed decision-making. After cleaning, the dataset was confirmed to be free of duplicates and was then loaded into Microsoft Excel for further analysis.

# Data Transformation
During the transformation phase, the key focus was on preparing the dataset for meaningful analysis, particularly around customer churn behavior.
The ‘Churn’ column, which indicates whether a customer has discontinued the service, was originally in text format (“Yes” or “No”). To allow for quantitative analysis, it was transformed into a numeric format — with “Yes” replaced by 1 and “No” by 0. This conversion ensured the column was summable and compatible with pivot tables and other analytical tools.
This transformation enabled the dataset to be more analysis-ready, ensuring the metrics could be used to derive insights into churn behavior, customer retention, and overall service performance.

# Data visualization 
Data Visualization was carried out using Microsoft Excel, where several pivot tables were created to summarize key metrics. Based on these, pivot charts were generated to provide visual insights into customer churn patterns.
The visualizations highlighted churn rate across various customer attributes, including contract type, partner status, internet service provider, age, and dependency status. Additionally, the charts illustrated the average monthly charges associated with each category, helping to uncover trends and support meaningful interpretation of customer behavior.

# Key Performance Indicators - KPIs
Total Customers - 7043. Churn Rate - 26.54%. Churn Customers - 1869. Retained Customers - 5174.
Month-to-month contracts have the highest churn rate at 42.7%, followed by one-year contracts at 11.3% and two-year contracts with the lowest at 2.8%. Churn rates range significantly depending on contract duration, with longer contracts resulting in lower churn rates. Customers on month-to-month contracts pay the highest average monthly fee of $66.40, followed by one-year contracts at $65.05, and two-year contracts with the lowest average monthly price of $60.77. Despite the disparity in churn rates, the average monthly prices vary very little between contract types.


