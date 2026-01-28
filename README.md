# Emotion Detection NLP Project


## Tech Stack
- Python
- Pandas, NLTK
- Scikit-learn
- TF-IDF, Bag of Words

## Models Used
- Naive Bayes
- Logistic Regression

## Dataset
Kaggle Emotion Dataset

## Features
- Text preprocessing pipeline
- Feature extraction using TF-IDF & BoW
- Model training and evaluation


## 1. Project Overview
This project is an NLP-based Emotion Detection system that classifies text into different emotions using Machine Learning models.

The main objective of this project is to understand how different text vectorization techniques (Bag of Words, TF-IDF) and ML models (Naive Bayes, Logistic Regression) affect model performance.

This project was built step-by-step with experimentation to find the best combination of features and models.

---

## 2. Problem Statement
Given a text sentence, predict the emotion expressed in the text.

Example:
Input: "I am feeling very happy today!"
Output: Happy 😊

---

## 3. Dataset
- Source: Kaggle Emotion Dataset
- Data Type: Text + Emotion Labels
- Classes: Multiple emotions (e.g., happy, sad, angry, fear, etc.)

---

## 4. Tools & Technologies Used

### Programming Language:
- Python

### Libraries:
- Pandas
- NLTK
- Scikit-learn

### NLP & ML Techniques:
- Text Preprocessing
- Bag of Words (CountVectorizer)
- TF-IDF (TfidfVectorizer)
- Naive Bayes
- Logistic Regression

---

## 5. Text Preprocessing Pipeline

The following preprocessing steps were applied:

1. Lowercasing text
2. Removing punctuation
3. Removing emojis
4. Removing stopwords
5. Tokenization
6. Text cleaning and normalization

Purpose:
To convert raw text into clean and meaningful data for ML models.

---

## 6. Model Building & Experiments

### Experiment 1: Bag of Words + Naive Bayes
- Vectorization: CountVectorizer (Bag of Words)
- Model: Naive Bayes
- Accuracy: 74%

Reason:
Naive Bayes performs well with frequency-based features.

---

### Experiment 2: TF-IDF + Naive Bayes
- Vectorization: TfidfVectorizer
- Model: Naive Bayes
- Accuracy: 61%

Observation:
Naive Bayes assumes feature independence and works better with raw frequency counts. TF-IDF weighting reduced its effectiveness.

---

### Experiment 3: TF-IDF + Logistic Regression (Best Model)
- Vectorization: TfidfVectorizer
- Model: Logistic Regression
- Accuracy: 81% ✅

Reason:
Logistic Regression handles weighted features better and captures linear relationships in text data.

---

## 7. Final Model Selection

Best performing model:
TF-IDF + Logistic Regression

Reason for selection:
- Highest accuracy (81%)
- Better generalization
- Suitable for weighted text features

---

## 8. Project Workflow

1. Data Collection (Kaggle)
2. Data Cleaning & Preprocessing
3. Feature Extraction (BoW & TF-IDF)
4. Model Training (Naive Bayes & Logistic Regression)
5. Model Evaluation
6. Performance Comparison
7. Final Model Selection

---


## Result
Achieved high accuracy in emotion classification.
And Hence the Logistic regression model has given the highest accuracy score using TF-Idf vectorization of 81%

## Author
Akash Soni


## 9. Folder Structure




emotion-sentiment-nlp/
│── dataset/
│── notebook.ipynb
│── requirements.txt
│── README.md
│── model/
│── src/
