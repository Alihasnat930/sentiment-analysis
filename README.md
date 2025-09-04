# Twitter/X Sentiment Analysis

This project classifies tweets as **Negative, Neutral, or Positive** using Machine Learning.

# 📊 Dataset

- ~75K tweets
- After cleaning: ~57K tweets
- Columns: `id`, `entity`, `sentiment`, `tweet`

Dataset: [Twitter Entity Sentiment Analysis](https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis)

# ⚙️ Workflow
1. Clean and preprocess tweets (remove links, mentions, hashtags, punctuation).
2. Convert text into numbers using **TF-IDF**.
3. Train a **Logistic Regression** model.
4. Evaluate with accuracy, precision, recall, and F1-score.

# 📈 Results
- Accuracy: **~79%**
- F1-scores:  
  - Negative: **0.82**  
  - Neutral: **0.76**  
  - Positive: **0.79**

[Sentiment distribution](./sentiment_distribution.png)
# 🔍 Example
tweet = "I love programming! #coding"
prediction = model.predict(vectorizer.transform([tweet]))
print(prediction)  # Positive
