# Project 6: Retail Analytics & Deep Learning Image Classification 🛍️

## 📌 Project Overview
Massive e-commerce platforms ingest millions of product images daily, making manual inventory categorization impossible. The goal of this project is to build a Computer Vision pipeline using Deep Learning. By training a Neural Network to interpret raw pixel matrices, we can automatically classify unstructured product images into distinct retail departments (e.g., footwear, apparel, accessories), streamlining the e-commerce tagging process.

## 📊 The Dataset
* **Source:** Kaggle Fashion-MNIST (Zalando Research)
* **Industry:** Retail / E-commerce
* **Description:** 60,000 training images and 12,000 testing images of retail products, mathematically flattened into 784-pixel arrays (28x28 grayscale resolution) across 10 distinct categories.

## 🛠️ Tools & Libraries Used
* **Language:** Python
* **Data Manipulation:** pandas, numpy
* **Deep Learning:** TensorFlow, Keras (Sequential, Dense, Dropout)
* **Data Visualization:** matplotlib (Image reconstruction, Learning Curves)
* **Environment:** Jupyter Notebook / Google Colab

## 💡 Visual Data Engineering
* **Mathematical Reconstruction:** Engineered a Python loop to extract the flattened 784-pixel arrays and mathematically reshape them back into 28x28 2D grids to visually verify the integrity of the unstructured visual data.
* **Matrix Normalization:** Scaled the raw pixel intensities (ranging from 0 to 255) down to a strict 0.0 - 1.0 range, ensuring mathematical stability and preventing gradient descent failure during the Neural Network training phase.

## 🧠 Deep Learning Architecture & Performance
* **The Neural Network:** Architected a fully connected Dense Neural Network featuring 101,770 trainable parameters. Utilized a 128-neuron hidden layer with a ReLU activation function to learn non-linear visual patterns, combined with a 20% Dropout layer to prevent algorithmic overfitting.
* **Classification Engine:** Deployed a 10-neuron output layer equipped with a Softmax activation function to calculate exact probability distributions across the inventory categories.
* **Model Convergence:** The AI achieved **~89% accuracy** on entirely unseen validation data. Evaluated the learning curves to visually prove the algorithm successfully generalized universal clothing shapes rather than memorizing the training data.
* **Live Visual Predictions:** Pushed hidden test matrices through the trained model, automatically reconstructing the pixels and color-coding the output to prove real-time classification success.
