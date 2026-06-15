# 🎬 Movie Genre Classification using Machine Learning

## 📌 Project Overview

This project was developed as part of the **CodSoft Machine Learning Internship**.

The objective of this project is to build a Machine Learning model that can automatically predict the genre of a movie based on its plot summary or textual description using Natural Language Processing (NLP) techniques.

---

## 🎯 Objective

To develop a movie genre classification system using:

- Natural Language Processing (NLP)
- TF-IDF Feature Extraction
- Machine Learning Classification Algorithms

The model predicts the most likely genre of a movie from its plot description.

---

## 📂 Dataset

The dataset contains movie information in TXT format with the following structure:

ID ::: Movie Title ::: Genre ::: Description

### Dataset Statistics

- Total Movies: **54,214**
- Total Genres: **27**
- No Missing Values

### Genres Included

- Action
- Adult
- Adventure
- Animation
- Biography
- Comedy
- Crime
- Documentary
- Drama
- Family
- Fantasy
- Game-Show
- History
- Horror
- Music
- Musical
- Mystery
- News
- Reality-TV
- Romance
- Sci-Fi
- Short
- Sport
- Talk-Show
- Thriller
- War
- Western

---

## 🛠️ Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Natural Language Processing (NLP)

---

## 📊 Exploratory Data Analysis (EDA)

The following analyses were performed:

- Dataset Inspection
- Missing Value Analysis
- Genre Distribution Analysis
- Description Length Analysis
- Data Visualization

---

## ⚙️ Feature Engineering

### TF-IDF Vectorization

TF-IDF (Term Frequency-Inverse Document Frequency) was used to convert movie descriptions into numerical feature vectors.

Parameters Used:

```python
TfidfVectorizer(
    stop_words='english',
    max_features=5000
)
```

This transformed textual movie descriptions into machine-readable numerical features.

---

## 🤖 Machine Learning Models Used

### 1. Multinomial Naive Bayes

A probabilistic machine learning algorithm commonly used for text classification tasks.

### 2. Logistic Regression

A supervised learning algorithm that achieved the highest performance on this dataset.

### 3. Support Vector Machine (Linear SVM)

A classification algorithm used to separate movie genres based on textual features.

---

## 📈 Model Performance

| Model | Accuracy |
|---------|---------:|
| Multinomial Naive Bayes | 52.32% |
| Logistic Regression | 57.95% |
| Linear SVM | 57.04% |

### 🏆 Best Model

**Logistic Regression**

Accuracy Achieved: **57.95%**

---

## 📋 Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Classification Report

---

## 🔍 Sample Prediction

Input:

```text
A haunted house is terrorized by evil spirits and mysterious murders.
```

Predicted Genre:

```text
Horror
```

---

## 💾 Model Saving

The trained model and TF-IDF vectorizer were saved using Pickle.

Generated Files:

- movie_genre_model.pkl
- tfidf_vectorizer.pkl

---

## 📁 Project Structure

```text
Task1_Movie_Genre_Classification
│
├── README.md
├── Movie_Genre_Classification.ipynb
├── Movie_Genre_Classification.py
├── movie_genre_model.pkl
└── tfidf_vectorizer.pkl
```

---

## 🎓 Learning Outcomes

Through this project, I gained practical experience in:

- Natural Language Processing (NLP)
- Text Preprocessing
- TF-IDF Feature Extraction
- Multi-Class Classification
- Machine Learning Model Evaluation
- Data Visualization
- Model Comparison

---

## 🚀 Future Improvements

Possible improvements include:

- Hyperparameter Tuning
- Advanced NLP Techniques
- Word Embeddings
- Deep Learning Models (LSTM, BERT)
- Handling Class Imbalance

---

## 🏁 Conclusion

A Movie Genre Classification system was successfully developed using NLP and Machine Learning techniques.

Three machine learning algorithms were trained and evaluated:

- Multinomial Naive Bayes
- Logistic Regression
- Linear SVM

Among all models, **Logistic Regression achieved the highest accuracy of 57.95%** and was selected as the final model.

This project demonstrates the practical application of NLP and Machine Learning for automated movie genre prediction.

---

## 👩‍💻 Author

**Radhika Suryawanshi**

CodSoft Machine Learning Internship – Task 1
