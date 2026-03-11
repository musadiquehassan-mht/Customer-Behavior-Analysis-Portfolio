# Project 7: Marketing Analytics & Unsupervised Customer Segmentation 🎯

## 📌 Project Overview
Mass-marketing campaigns are highly inefficient and costly. The objective of this project is to leverage Unsupervised Machine Learning to discover hidden demographic patterns within a banking database. By deploying a K-Means Clustering algorithm, we mathematically grouped over 11,000 unstructured customer profiles into distinct target audiences based on age and financial behavior, enabling data-driven, personalized marketing strategies.

## 📊 The Dataset
* **Source:** Bank Marketing Dataset (Kaggle)
* **Industry:** Marketing / Advertising / Finance
* **Description:** 11,163 customer records detailing demographic information (age, job, marital status) and financial metrics (account balance, loan status, campaign interactions).

## 🛠️ Tools & Libraries Used
* **Language:** Python
* **Data Manipulation:** pandas
* **Data Preprocessing:** scikit-learn (StandardScaler)
* **Machine Learning:** scikit-learn (K-Means Clustering)
* **Data Visualization:** matplotlib, seaborn (Scatterplots, The Elbow Method)
* **Environment:** Jupyter Notebook / Google Colab

## ⚙️ Engineering & Methodology
* **Feature Scaling:** Isolated numerical target features (`age` and `balance`). Deployed a `StandardScaler` to force a mean of 0 and a standard deviation of 1, preventing variables with massive absolute values (like bank balances) from mathematically overpowering smaller variables (like age) during distance calculations.
* **The Elbow Method:** Iterated the K-Means algorithm for $k=1$ through $k=10$ clusters. Calculated the Within-Cluster Sum of Squares (WCSS) to mathematically identify the optimal number of target audiences before encountering diminishing returns. The algorithm confirmed 4 distinct customer segments.
* **Unsupervised Clustering:** Initialized the K-Means engine with `k-means++` to optimize centroid convergence. The AI successfully calculated the Euclidean distance across the feature space, assigning every customer a strict `Target_Audience` ID.

## 📈 Engine Diagnostics & Business Insights
Because Unsupervised Learning lacks true labels, traditional accuracy metrics cannot be applied. The algorithm's structural integrity was evaluated using the **Silhouette Score**, achieving a **0.53** (a highly positive score indicating well-separated, distinct clusters for real-world human behavior data).

By aggregating the original financial data against the AI's structural predictions, we extracted four actionable Marketing Personas for immediate campaign deployment:

1. **The Starters (Target 1):** Average Age 33.8 | Average Balance $767. (Prime targets for entry-level credit and auto loans).
2. **The Savers (Target 2):** Average Age 41.5 | Average Balance $7,575. (Targets for premium checking and investment portfolios).
3. **The Established (Target 0):** Average Age 54.8 | Average Balance $1,111. (Targets for fixed-rate mortgages and retirement products).
4. **The Whales (Target 3):** Average Age 48.5 | Average Balance $28,855. (High-net-worth outliers targeted for VIP wealth management).
