# 🎬 Sentiment Analysis on IMDB Movie Reviews

This project implements a **Sentiment Analysis model** to classify IMDB movie reviews as **Positive** or **Negative** using Natural Language Processing (NLP) and Machine Learning.

---

## 📌 Dataset

- Dataset: IMDB Movie Reviews
- Source: Kaggle
- Size: 50,000 movie reviews
- Labels: `positive`, `negative`

Dataset used:
https://www.kaggle.com/datasets/vishakhdapat/imdb-movie-reviews

---

## 🧹 Data Preprocessing

The following preprocessing steps were applied:

- Lowercasing text
- Removing HTML tags
- Removing punctuation & numbers
- Stopwords removal (NLTK)
- Removing duplicate reviews
- Mapping labels:
  - Positive → 1
  - Negative → 0

---

## 📊 Exploratory Data Analysis (EDA)

- Checked null & duplicated values
- Visualized sentiment distribution
- Extracted most frequent positive & negative words using:
  - VADER Sentiment Analyzer
  - Word frequency analysis

---

## 🔤 Feature Engineering

Vectorization method:

- **TF-IDF**
  - max_features = 30,000
  - ngram_range = (1,2)

---

## 🤖 Models Used

Two machine learning models were trained and compared:
1. Logistic Regression
2. Multinomial Naive Bayes

### 📈 Evaluation Metrics

- Accuracy
- Classification Report (Precision, Recall, F1-score)
- Confusion Matrix
- Model comparison visualization

---

## 🏆 Results

Logistic Regression outperformed Naive Bayes in accuracy.

The final deployed model: **Logistic Regression**

---

## 🔮 Prediction Function

You can test custom reviews using:

```python
predict_sentiment("This movie was absolutely amazing")
predict_sentiment("Worst film I have ever watched")
