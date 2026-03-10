# Project 4: Streaming Industry NLP Sentiment Analysis 🍿

## 📌 Project Overview
In the streaming and entertainment industry, manually reading millions of user reviews to gauge audience satisfaction is impossible. The goal of this project is to build a Natural Language Processing (NLP) pipeline that automatically ingests raw, unstructured movie reviews, cleans the text, and utilizes a Machine Learning algorithm to classify the underlying human sentiment as either Positive or Negative.

## 📊 The Dataset
* **Source:** Kaggle IMDB 50K Movie Reviews
* **Industry:** Streaming / Entertainment
* **Description:** 50,000 raw text reviews from audience members, perfectly balanced with 25,000 positive and 25,000 negative labels.

## 🛠️ Tools & Libraries Used
* **Language:** Python
* **Text Processing:** Regular Expressions (re), Natural Language Toolkit
* **Data Visualization:** matplotlib, seaborn, wordcloud
* **Machine Learning:** scikit-learn (TF-IDF Vectorizer, Logistic Regression)
* **Environment:** Jupyter Notebook / Google Colab

## 💡 NLP Pipeline & Exploratory Insights
* **Text Scrubbing:** Engineered a custom Python cleaning function to strip out raw HTML tags (e.g., `<br />`), remove non-alphabetical punctuation, and standardize all text to lowercase to ensure mathematical consistency.
* **Emotional Vocabulary Visualization:** Deployed custom Word Clouds equipped with "Stopword" filters (removing generic terms like 'the', 'movie', and 'film') to isolate the primary drivers of satisfaction (e.g., "great", "best") versus dissatisfaction (e.g., "bad", "worst").

## 🤖 Predictive Modeling: Text-to-Math Vectorization
* **TF-IDF Transformation:** Converted the unstructured English vocabulary into a mathematical matrix using Term Frequency-Inverse Document Frequency (TF-IDF), assigning mathematical weights to the 5,000 most predictive words.
* **Logistic Regression Engine:** Trained a classification algorithm on the vectorized text, achieving a highly accurate **89.5% success rate** on unseen testing data.
* **Live Testing:** Deployed a custom Python function capable of taking brand new, real-time string inputs, pushing them through the scrubber and vectorizer, and accurately predicting the sentiment on the fly.
