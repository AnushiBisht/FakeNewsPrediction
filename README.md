# 📰 Fake News Prediction using Machine Learning

A machine learning project that detects whether a news article is **Real** or **Fake** using **Natural Language Processing (NLP)** and a **Logistic Regression** model.  
Built with Python, Scikit-learn, NLTK, and TF-IDF vectorization.

---

## 🚀 Features

- ✅ News article classification (Real or Fake)
- ✅ Text preprocessing and cleaning
- ✅ Stopword removal using NLTK
- ✅ Stemming using PorterStemmer
- ✅ TF-IDF vectorization
- ✅ Logistic Regression model training
- ✅ Accuracy evaluation
- ✅ Predict custom news input

---

## 🛠️ Tech Stack

- **Python**
- **Pandas**
- **NumPy**
- **NLTK**
- **Scikit-learn**
- **Jupyter Notebook**

---

## 📂 Dataset

This project uses two CSV datasets:

- `True.csv` → Contains real news articles
- `Fake.csv` → Contains fake news articles

The datasets are merged and labeled:

| Label | Meaning |
|-------|---------|
| 1 | Real News |
| 0 | Fake News |

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/fake-news-prediction.git
cd fake-news-prediction
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Download NLTK Stopwords

```python
import nltk
nltk.download('stopwords')
```

---

## ▶️ Run the Project

Start Jupyter Notebook:

```bash
jupyter notebook fakeNewsPrediction.ipynb
```

Run all notebook cells to:

1. Load and preprocess the dataset
2. Convert text into vectors
3. Train the ML model
4. Evaluate accuracy
5. Predict fake or real news

---

## 🧠 Machine Learning Workflow

### 📌 1. Data Preprocessing

The text data is cleaned by:
- Removing punctuation and special characters
- Converting text to lowercase
- Removing stopwords
- Applying stemming

Example:

```python
from nltk.stem.porter import PorterStemmer
```

---

### 📌 2. Feature Extraction

TF-IDF Vectorizer converts textual data into numerical vectors.

```python
from sklearn.feature_extraction.text import TfidfVectorizer

vectorizer = TfidfVectorizer()
```

---

### 📌 3. Model Training

A Logistic Regression classifier is used for prediction.

```python
from sklearn.linear_model import LogisticRegression

model = LogisticRegression()
```

---

### 📌 4. Model Evaluation

The model performance is evaluated using:
- Training Accuracy
- Testing Accuracy

---

## 📊 Sample Prediction

```python
prediction = model.predict(X_new)

if prediction == 1:
    print("Real News")
else:
    print("Fake News")
```

---

## 📁 Project Structure

```bash
fake-news-prediction/
│
├── fakeNewsPrediction.ipynb
├── Fake.csv
├── True.csv
├── README.md
└── requirements.txt
```

---

## 📌 Future Improvements

- 🌐 Build a Flask/FastAPI web application
- 🚀 Deploy the model online
- 🧠 Use Deep Learning models like:
  - LSTM
  - GRU
  - BERT
- 📡 Add real-time news article prediction
- 📱 Create a frontend UI

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a new branch
3. Commit your changes
4. Push the branch
5. Open a Pull Request

---

## 👨‍💻 Author

**Anushi Bisht**

If you liked this project, give it a ⭐ on GitHub!
