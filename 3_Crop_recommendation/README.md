# Project 3: Precision Agriculture & Crop Recommendation System 🌾

## 📌 Project Overview
Precision agriculture relies on data-driven decision-making to maximize crop yield and optimize resource usage. This project transitions from analyzing human behavioral data to processing precise environmental IoT sensor data. The goal is to build a Multiclass Machine Learning recommendation engine that automatically determines the optimal crop for a specific farm based on soil nutrients and climate metrics.

## 📊 The Dataset
* **Source:** Kaggle Crop Recommendation Dataset
* **Industry:** Agriculture / IoT Sensor Data
* **Description:** A perfectly balanced dataset containing 2,200 sensor readings across 22 distinct crop types. Features include Nitrogen (N), Phosphorus (P), Potassium (K), pH levels, temperature, humidity, and rainfall.

## 🛠️ Tools & Libraries Used
* **Language:** Python
* **Data Manipulation:** pandas
* **Data Visualization:** matplotlib, seaborn (Correlation Heatmaps, Boxplots)
* **Machine Learning:** scikit-learn (Random Forest Classifier)
* **Environment:** Jupyter Notebook / Google Colab

## 💡 Key Insights Uncovered (EDA)
* **Perfect Target Balance:** Verified the dataset was perfectly balanced (exactly 100 readings per crop), preventing the algorithm from developing predictive bias.
* **Nutrient Signatures:** Mapped out distinct mathematical "footprints" for each crop using boxplots (e.g., Cotton demands extreme Nitrogen levels, while legumes require almost none).
* **Environmental Correlations:** Identified strong natural correlations in the soil data, specifically a 0.74 positive correlation between Phosphorus (P) and Potassium (K).

## 🤖 Predictive Modeling: Multiclass Classification
* **Algorithm:** Deployed a Random Forest Classifier to learn the 22 distinct crop signatures.
* **Performance:** Because sensor data represents precise physical metrics rather than unpredictable human behavior, the model achieved a phenomenal **99.3% Accuracy** on unseen testing data.
* **Feature Importance:** Extracted the algorithmic weights to prove that **Rainfall** and **Humidity** are the ultimate deciding factors for crop viability, mathematically outweighing manually adjustable soil nutrients.
