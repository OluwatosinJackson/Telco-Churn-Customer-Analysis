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

To support churn analysis, three new columns were created:

    Churn Count: Derived using the formula =IF([@Churn]="No", 0, 1), this column flags churned customers with a 1 and retained customers with a 0.

    Customer Count: Calculated using the formula =COUNTIF([customerID], [@customerID]), this ensures each customer is counted accurately for total customer metrics.

Churn Rate and Non-Churn Customers: These were added as calculated fields in the PivotTable.

    Churn Rate = Churn Count ÷ Customer Count

    Non-Churn Customers = Customer Count - Churn Count

These transformations enabled the dataset to be more analysis-ready, ensuring the metrics could be used to derive insights into churn behavior, customer retention, and overall service performance.
