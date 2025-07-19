# Zomato_Restaurant_Clustering_and_Sentiment_Analysis
---

## 📚 Table of Contents
- [📌 Introduction](#introduction)
- [📊 Project Overview](#project-overview)
- [🧹 Preprocessing Data](#preprocessing-data)
- [🛠️ Feature Engineering](#feature-engineering)
- [🤖 ML Model Implementation](#ml-model-implementation)
- [✅ Conclusion](#conclusion)

---

## 📌 Introduction

This project is a part of my Machine Learning Capstone and demonstrates real-world application of data science techniques on Zomato datasets. It includes advanced text preprocessing, feature extraction, clustering analysis using K-Means, and topic modeling using LDA (Latent Dirichlet Allocation).

---

## 📊 Project Overview

- **Data Collection:** Collected datasets containing restaurant details and customer reviews.
- **Data Preprocessing:** Performed cleaning, formatting, and normalization to prepare the data for ML models.
- **Feature Engineering:** Created new features, transformed existing ones, and performed sentiment tagging.
- **ML Models:** Implemented K-Means clustering and LDA to group and analyze restaurants and review content.
- **Model Evaluation:** Assessed performance using metrics such as Silhouette Score, ROC AUC, Precision, Recall, etc.

---

## 🧹 Preprocessing Data

- Merged restaurant and review data for analysis.
- Cleaned missing values, nulls, and inconsistencies.
- Performed advanced text preprocessing:
  - Lowercasing
  - Removal of punctuation, digits, URLs
  - Stopword removal
  - Contraction expansion
- Applied `nltk`, `spaCy`, and `sklearn` utilities for tokenization and vectorization.

---

## 🛠️ Feature Engineering

- Engineered new columns from review text using TF-IDF, sentiment scores, and word counts.
- Labeled sentiment based on review rating (positive, neutral, negative).
- Applied log transformation to normalize skewed features like `Cost`.
- Minimized multicollinearity and selected high-impact features for modeling.

---

## 🤖 ML Model Implementation

### 1. **K-Means Clustering**
- Grouped restaurants into 6 clusters based on textual and numerical features.
- Visualized clusters using PCA and evaluated using **Silhouette Score**.

### 2. **Latent Dirichlet Allocation (LDA)**
- Applied LDA for unsupervised topic modeling on customer reviews.
- Extracted top terms and topic distributions for insights.
- Visualized results using `pyLDAvis`.

---

## ✅ Conclusion

- Achieved meaningful segmentation of restaurants using K-Means.
- LDA revealed key topics in customer sentiment (e.g., food quality, service, ambiance).
- Optimized `n_components` using Silhouette Score for clustering and coherence for LDA.
- This end-to-end pipeline offers a powerful framework for deriving insights from textual and structured data in the food tech industry.

---

### 📌 Future Work
- Apply BERT or transformer-based models for more accurate sentiment classification.
- Develop a recommendation system using collaborative filtering or NLP embeddings.
- Deploy models in a Flask app for real-time predictions and dashboard integration.
"""
