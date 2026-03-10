# Project 5: Healthcare Analytics & Medical Cost Regression 🏥

## 📌 Project Overview
In the insurance industry, profitability relies on precise mathematical risk assessment. The goal of this project is to analyze patient demographics and health metrics to determine the primary drivers of medical costs. We transitioned from classification tasks to building a Machine Learning Regression engine capable of predicting exact, continuous dollar amounts for annual medical charges, allowing for automated, dynamic insurance premium pricing.

## 📊 The Dataset
* **Source:** Kaggle Medical Cost Personal Datasets
* **Industry:** Healthcare / Insurance
* **Description:** 1,338 patient records containing demographic data (age, sex, region) and health metrics (BMI, children, smoking status) mapped against their annual medical charges.

## 🛠️ Tools & Libraries Used
* **Language:** Python
* **Data Manipulation:** pandas
* **Data Visualization:** matplotlib, seaborn (Histograms, Multivariate Scatterplots, Boxplots)
* **Machine Learning:** scikit-learn (Random Forest Regressor, One-Hot Encoding)
* **Environment:** Jupyter Notebook / Google Colab

## 💡 Key Insights Uncovered (EDA)
* **Cost Distribution:** Verified that annual medical costs are heavily right-skewed, with the majority of patients incurring routine costs under $15,000, while a high-risk subset experiences catastrophic charges exceeding $40,000.
* **The Financial Impact of Smoking:** Isolated smoking status to visually prove that the absolute minimum medical bill for a smoker is significantly higher than the median bill for a non-smoker.
* **Compounding Risk Factors:** Mapped a multivariate scatterplot revealing a non-linear pricing structure: while BMI has a gradual impact on non-smokers, hitting a BMI of 30 (obesity) as a smoker triggers a massive, catastrophic spike in medical charges.

## 🤖 Predictive Modeling: Random Forest Regression
* **Data Preparation:** Engineered a categorical text-to-math pipeline using Pandas `get_dummies` (One-Hot Encoding) to translate text features (`sex`, `smoker`, `region`) into binary matrices while avoiding the dummy variable trap.
* **Algorithm:** Deployed a Random Forest Regressor specifically chosen for its ability to handle sudden, non-linear compounding spikes in the data.
* **Performance:** The regression engine successfully explained **86.51% of the financial variance (R-squared)** with a highly competitive Mean Absolute Error (MAE) given the extreme outliers in catastrophic medical billing.
* **Feature Importance:** Extracted the algorithmic weights to prove to actuaries that smoking status mathematically outweighs all other metrics combined when forecasting financial risk.
