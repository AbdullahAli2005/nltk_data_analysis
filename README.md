# NLTK Movie Review Sentiment Analysis

This project demonstrates a **basic sentiment analysis system** using **NLTK** and a **Naive Bayes classifier**. The model is trained on the built-in `movie_reviews` dataset and can predict whether a given sentence expresses a **positive** or **negative** sentiment.

---

## 📌 Overview

The application:

* Uses NLTK’s `movie_reviews` corpus as training data
* Applies basic text preprocessing (tokenization and stopword removal)
* Trains a Naive Bayes classifier
* Evaluates model accuracy
* Predicts sentiment for custom input sentences

This project is suitable for **learning NLP fundamentals** and understanding how classical machine learning models work in text classification.

---

## 🛠️ Technologies Used

* Python 3
* NLTK (Natural Language Toolkit)
* Naive Bayes Classifier

---

## 📂 Project Structure

```
nltk_data_analysis/
│
├── main.py        # Main script for training and testing sentiment model
├── README.md      # Project documentation
└── .venv/         # Python virtual environment (optional)
```

---

## ⚙️ Installation & Setup

### 1. Create and activate a virtual environment (optional but recommended)

```bash
python -m venv .venv
.venv\Scripts\activate   # Windows
```

### 2. Install dependencies

```bash
pip install nltk
```

---

## 📥 NLTK Data Downloads

The script automatically downloads the required NLTK datasets on first run:

* `movie_reviews`
* `punkt`
* `punkt_tab`
* `stopwords`

No manual download is required.

---

## ▶️ How to Run

Execute the script using:

```bash
python main.py
```

---

## 📊 Output Details

### Model Accuracy

The script prints classification accuracy on the test dataset, for example:

```
Accuracy: 65.50%
```

### Most Informative Features

The classifier displays words that are most strongly associated with positive or negative sentiment:

```
outstanding = True   pos : neg = 13.2 : 1.0
sucks       = True   neg : pos = 14.3 : 1.0
```

### Sentiment Prediction

The model predicts sentiment for custom sentences:

```
Sentence: This movie is absolutely fantastic!
Predicted sentiment: pos
```

---

## 🧠 How It Works

1. **Tokenization** – Text is split into words using NLTK’s tokenizer
2. **Stopword Removal** – Common English stopwords are removed
3. **Feature Extraction** – Each word is treated as a boolean feature
4. **Training** – Naive Bayes model is trained on labeled movie reviews
5. **Prediction** – New sentences are classified as `pos` or `neg`

---

## 🚀 Possible Improvements

* Use TF-IDF instead of binary word features
* Add bigram or trigram features
* Apply stemming or lemmatization
* Replace Naive Bayes with Logistic Regression or SVM
* Build a web or REST API interface

---

## 📚 Learning Purpose

This project is intended for **educational use** and is ideal for:

* Beginners learning NLP
* Understanding classical ML approaches to sentiment analysis
* Experimenting with NLTK corpora and classifiers

---

## 📝 License

This project is open-source and free to use for learning and experimentation.
