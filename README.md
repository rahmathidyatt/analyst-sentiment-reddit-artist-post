# Sentiment Analysis of Reddit Artist Posts using Naive Bayes

This project implements a sentiment analysis pipeline to classify Reddit posts
related to artists into sentiment categories using a machine learning approach.
The workflow combines TF-IDF feature extraction, SMOTE for handling class
imbalance, and a Naive Bayes classifier.

---

## 📌 Overview

Sentiment analysis is a text mining technique used to identify and classify
opinions or emotions expressed in textual data. In this project, Reddit posts
related to artists are analyzed and classified into sentiment labels using a
supervised machine learning model.

The main objective of this project is to build a reproducible and interpretable
sentiment classification pipeline suitable for academic study and portfolio use.

---

## 📂 Dataset

The dataset used in this project was obtained from **Kaggle**.
It consists of Reddit posts related to artists along with sentiment labels.
The dataset is publicly available and used solely for research and educational
purposes.

> **Note:** The exact dataset author on Kaggle is not specified in this repository.
> The dataset is treated as a public benchmark for sentiment analysis experiments.

---

## 🛠 Methodology

The analysis follows a structured machine learning pipeline:

1. **Data Preparation**
   - Loading Reddit post data from CSV format
   - Encoding sentiment labels into numerical values

2. **Train–Test Split**
   - 80% training data
   - 20% testing data

3. **Feature Extraction**
   - TF-IDF (Term Frequency–Inverse Document Frequency)

4. **Class Imbalance Handling**
   - SMOTE (Synthetic Minority Over-sampling Technique) applied only to training data

5. **Model Training**
   - Multinomial Naive Bayes classifier

6. **Model Evaluation**
   - Accuracy
   - Classification Report
   - Confusion Matrix and Heatmap Visualization.

---

## 📊 Results

The Naive Bayes model achieved the following performance on the test dataset:

- **Accuracy:** **67.76%**

### Classification Summary
- The model performs well on the **neutral** class, which represents the majority
  of the dataset.
- Recall for the **negative** class is relatively high, indicating that most
  negative sentiments are successfully detected.
- The **positive** class shows balanced precision and recall, demonstrating
  reasonable predictive capability.

Overall, the results indicate that the combination of **TF-IDF**, **SMOTE**, and
**Naive Bayes** is effective for sentiment classification on Reddit artist-related
text data, while still leaving room for improvement through more advanced models
or hyperparameter tuning.

---

## 🧰 Tools & Libraries

- Python 3
- pandas
- scikit-learn
- imbalanced-learn (SMOTE)
- matplotlib
- seaborn

---

## 📁 Repository Structure

analyst-sentiment-reddit-artist-post/
│
├── dataset/
│ └── reddit_artist_posts_sentiment.csv
│
├── naive bayes.ipynb
└── README.md

---

## 👤 Author

**Rahmat Hidayat**  
