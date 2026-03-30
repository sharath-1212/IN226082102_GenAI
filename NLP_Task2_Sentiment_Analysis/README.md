#  Sentiment Analysis using NLP Pipeline & Machine Learning

##  Project Overview
This project demonstrates a complete end-to-end Sentiment Analysis system built using Natural Language Processing (NLP) techniques and Machine Learning models. The primary objective is to convert raw text data into structured numerical features and classify sentiments (positive/negative) accurately.

---

##  Objectives
- Understand and implement NLP preprocessing techniques
- Convert textual data into machine-understandable features
- Train multiple Machine Learning models
- Evaluate and compare model performance using standard metrics

---

##  Dataset
- Source: Kaggle (IMDb Reviews / Amazon Reviews / Twitter Sentiment Dataset)
- The dataset contains text samples labeled with sentiments such as positive or negative.

---

##  Tech Stack
- **Language:** Python  
- **Libraries:**
  - pandas – Data manipulation
  - numpy – Numerical operations
  - nltk – Natural Language Processing
  - re – Regular expressions for text cleaning
  - scikit-learn – Machine Learning models & evaluation

---

##  NLP Pipeline

### 1️ Text Preprocessing
Text preprocessing is crucial to clean and standardize raw data before feeding it into machine learning models.

Steps involved:
- Lowercasing text
- Removing punctuation and special characters
- Tokenization (splitting text into words)
- Stopword removal (removing common words like "the", "is")
- Lemmatization (reducing words to their base form)

Example:
Input: "I loved this movie! It's amazing."
Output: ["love", "movie", "amazing"]

---

### 2️ Feature Engineering
Transforming text into numerical vectors:

- **Bag of Words (BoW):**
  Converts text into word frequency vectors.

- **TF-IDF (Term Frequency - Inverse Document Frequency):**
  Weighs words based on importance rather than frequency.

---

### 3️ Model Building
The following Machine Learning models were trained:

- Logistic Regression  
- Multinomial Naive Bayes  
- Decision Tree Classifier  

Each model learns patterns from the processed text data to predict sentiment.

---

### 4️ Model Evaluation
Models were evaluated using:

- Accuracy – Overall correctness  
- Precision – Correct positive predictions  
- Recall – Coverage of actual positives  
- F1-Score – Balance between precision and recall  

---

##  Results
- Compared performance of all models
- Observed that preprocessing significantly improves accuracy
- TF-IDF generally performs better than Bag of Words
- Identified the best-performing model based on evaluation metrics

---

