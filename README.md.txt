# 📰 Fake News Detection Using Machine Learning

This project uses machine learning to detect fake news based on news headlines. It utilizes natural language processing (NLP), TF-IDF vectorization, and classification models such as Logistic Regression and Naive Bayes.

---

## 📁 Dataset

- Source: `FakeNewsNet.csv`  
- Columns: `title`, `news_url`, `source_domain`, `tweet_num`, `real`
- Binary labels:  
  - `1` = Real News  
  - `0` = Fake News

---

## 🔧 Technologies Used

- Python
- Jupyter Notebook
- pandas, numpy
- nltk (for text preprocessing)
- scikit-learn (for ML models and metrics)
- matplotlib & seaborn (for visualization)

---

## 📊 Project Steps

### 1. Data Cleaning & Preprocessing
- Remove nulls
- Rename column `real` → `label`
- Apply text cleaning:
  - Remove links, punctuation, and stopwords
  - Convert to lowercase

### 2. TF-IDF Vectorization
- Convert cleaned text into numerical format

### 3. Model Building
- **Logistic Regression**: Baseline model
- **Naive Bayes**: Added for comparison

### 4. Evaluation
- Accuracy score
- Classification report (Precision, Recall, F1)
- Confusion matrix heatmap

### 5. Predict Your Own Headlines
- A custom `predict_news("Your headline here")` function

---

## 🧠 Example

```python
predict_news("Breaking: Government launches new education scheme")
