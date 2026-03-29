# PSL Twitter Sentiment Analysis (Python)

## 📌 Objective

Build an end-to-end data pipeline to analyze Twitter data, extract user behavior patterns, and predict tweet sentiment using natural language processing (NLP) and machine learning.

---

## 📊 Dataset

* Source: Twitter Streaming API (PSL Final 2022)
* Size: ~8,300 tweets
* Includes tweet text, user metadata, engagement metrics, and hashtags

A sample dataset (`tweets_sample.csv`) is included for demonstration. The full dataset (~35MB) is available upon request.

---

## 🧹 Data Processing & Feature Engineering

### Data Cleaning:

* Extracted relevant tweet and user-level features
* Removed URLs, mentions, hashtags, and noise from text
* Standardized column names and formats

### Text Processing:

* Translated non-English tweets into English using Google Translate API
* Generated cleaned text for analysis

### Feature Engineering:

* Extracted hashtags, mentions, and engagement metrics
* Created sentiment labels using VADER sentiment analysis

---

## 📈 Exploratory Data Analysis

Key analyses performed:

* Tweet volume over time
* Sentiment trends vs activity
* User engagement patterns
* Geographic tweet distribution
* Hashtag frequency (word cloud visualization)

---

## 🤖 Machine Learning

### 1. Sentiment Classification

* **Technique:** TF-IDF + Logistic Regression
* Converted text into 5,000-dimensional feature vectors
* Classified tweets into:

  * Positive
  * Neutral
  * Negative

**Performance:**

* Accuracy: ~76%
* Strong performance on positive sentiment
* Lower recall for negative class

---

### 2. User Segmentation (Clustering)

* **Method:** K-Means Clustering

* Features used:

  * Followers
  * Friends
  * Favorites
  * Status count

* Applied log transformation for normalization

**Clusters Identified:**

* Casual users
* Moderate users
* Highly active / influential users

---

### 3. Dimensionality Reduction

* **Technique:** Principal Component Analysis (PCA)
* Used to visualize cluster separation in 2D space

---

## 🔍 Model Evaluation

* Classification report (precision, recall, F1-score)
* Confusion matrix visualization
* Cluster distribution analysis

---

## 🛠️ Tools & Libraries

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn
* WordCloud
* Deep Translator (Google Translate)

---

## 📌 Key Insights

* Positive sentiment dominates Twitter activity in the dataset
* High tweet volume often correlates with neutral or mixed sentiment
* Highly active users form a distinct cluster with strong engagement
* Hashtags reveal trending topics and user interests

---

## 🚀 Key Takeaway

This project demonstrates how unstructured social media data can be transformed into actionable insights using data cleaning, NLP, machine learning, and visualization techniques.


