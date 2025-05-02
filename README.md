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
This analysis explores key factors influencing customer churn, with a focus on a number of factors. The dataset consists of 7,043 customers, with a churn rate of 26.54% — translating to 1,869 churned customers and 5,174 retained customers.
Month-to-month contracts have the highest churn rate at 23.5%, followed by one-year contracts at 2.36% and two-year contracts with the lowest at 0.88%. Churn rates range significantly depending on contract duration, with longer contracts resulting in lower churn rates. Customers on month-to-month contracts pay the highest average monthly fee of $66.40, followed by one-year contracts at $65.05, and two-year contracts with the lowest average monthly price of $60.77. Despite the disparity in churn rates, the average monthly prices vary very little between contract types.

Electronic Check methods was the most common method of payment amoong Customers as about 33.58% of the customer uses this payment method, 22.89% uses mail check, 21.92% and 21.61% using bank transfers and credit cards respectively. Electronic check methods have the highest churn rate at 57.30%.

The Internet service provider was a determinant on the churn rate of customers, as it was observed that fiberone which had the highest percentage of customers at 43.96% also had the highest churn rate at 69.40%. This high churn rate can be attributed to the its average monthly cost as was observed that it had the highest monthly average cost @ N91.50.

Customers with partners have a reduced churn rate of 9.50%, whereas those without partners have a higher churn rate (17.0%). This shows that having a partner is associated with a lower chance of churn. Customers with partners pay an average monthly charge of N67.78, compared to N61.95 for those without partners. Despite their differences, both groups contribute to the aggregate average monthly charge of N64.76.

Most customers are not senior Citizens, as only 16.21% of customer is 65 years of older. However the Churn rate is higher with senior citizens.

Customers without dependents have a greater churn rate (21.91%) than those with dependents (4.635%). Customers who have dependents have lower churn rates. 

# Recommendations
Contracts category: Giving discount and other incentives will encourage customers to opt for longer term contracts, which on the long run will help reduce the rate at whoch customers churn. Improving the value proposition for month-to-month subscribers and strategically upselling them to one-year contracts can further bolster retention efforts. Ensuring satisfaction across all contract types is crucial for maintaining long-term customer relationships. 
Partnership with Internet Service Providers category: it is important to ensure that internet service providers are help accountable for the services given to customers, such that customers paying high avergae monthly costs enjoy the benefits of what is being paid for, this will help also help to reduce churn.
Senior Citizens Category: providing specialized offers and services tailored to this demographic can foster loyalty and retention. Enhancing the perceived value of subscriptions for senior citizens, along with offering personalized support and assistance, can help address their unique needs. Tailoring marketing messages to resonate with seniors and senior citizens can further enhance engagement and retention efforts. Dependents category: providing targeted discounts and services for customers with dependents can foster loyalty, while enhancing the value proposition for those without dependents can justify their subscription costs. Offering educational resources and support for customers with dependents can help them maximize the benefits of their subscriptions. Tailoring marketing strategies to address the unique needs of each group within this category can further strengthen retention efforts.



