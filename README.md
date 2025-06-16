# 📰 Fake News Detection using Machine Learning

A simple yet effective machine learning project that detects whether a news headline is **fake** or **real** using NLP techniques.

---

## 📂 Dataset
- Source: `FakeNewsNet.csv`
- Columns used: `title` (text input), `real` (target label)

---

## 🧠 Model Workflow

1. **Text Cleaning & Preprocessing**
   - Lowercase, remove punctuation, stopwords
   - Tokenization + Lemmatization (NLTK)
2. **Vectorization**
   - TF-IDF Vectorizer (max 5000 features)
3. **Model Training**
   - Logistic Regression (baseline)
   - Optional: Naive Bayes / Random Forest
4. **Evaluation**
   - Accuracy, Confusion Matrix, Classification Report
5. **Prediction**
   - Custom headline input for real-time prediction

---

## 📊 Results

| Metric      | Score     |
|-------------|-----------|
| Accuracy    | `~93%`    |
| Precision   | `High`    |
| Recall      | `High`    |
| F1 Score    | `Balanced`|

---

## 🔍 Sample Usage

```python
predict_news("Government launches new healthcare program")
# Output: Real
