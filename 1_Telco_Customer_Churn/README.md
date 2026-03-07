Project 1: Telco Customer Churn Analysis 📉
📌 Project Overview
Customer retention is one of the most critical metrics for any subscription-based business. The goal of this project is to analyze customer behavior in the telecommunications sector to identify the primary drivers of customer churn (cancellation of service). By understanding who is leaving and why, we can provide data-driven recommendations to improve retention rates.

📊 The Dataset
Source: IBM Telco Customer Churn Dataset

Industry: Telecommunications

Description: The dataset contains demographics, account information, and service usage details for over 7,000 customers, alongside their final churn status.

🛠️ Tools & Libraries Used
Language: Python

Data Cleaning & Manipulation: pandas

Data Visualization: matplotlib, seaborn

Environment: Jupyter Notebook / Google Colab

💡 Key Insights Uncovered
Through Exploratory Data Analysis (EDA) and correlation mapping, several major risk factors were identified:

The Contract Trap: Customers on Month-to-Month contracts churn at a significantly higher rate than those on 1-year or 2-year contracts.

The New Customer Flight Risk: There is a strong negative correlation between tenure and churn (-0.35). Customers are highly likely to leave within their first 10 months. If they survive the first year, their loyalty increases dramatically.

The Premium Service Paradox: Fiber Optic internet customers churn at a much higher rate than DSL customers, despite having a faster connection. This suggests potential pricing or reliability issues.

The Tech Support Lifeline: Customers lacking Tech Support have the highest churn rates across all service categories. Providing tech support dramatically reduces the likelihood of a customer leaving.

🚀 Business Recommendations
Based on the mathematical findings, the telecom company should implement the following strategies to reduce churn:

Targeted Tech Support: Offer discounted or free tech support to new customers, specifically those signing up for Fiber Optic internet.

Incentivize Long-Term Contracts: Create aggressive promotions or discount structures that encourage month-to-month customers to lock in 1-year contracts, as crossing the 12-month tenure threshold significantly drops churn probability.

Investigate Fiber Optic Infrastructure: Conduct further analysis on customer support tickets for Fiber Optic users to determine if the high churn is due to network outages or perceived lack of value for the high monthly charge.
