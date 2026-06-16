# 💳 Credit Card Fraud Detection Using Machine Learning

An end-to-end machine learning classification framework engineered to identify anomalous patterns and detect fraudulent credit card transactions in real-time. This system handles real-world, highly imbalanced transaction matrices by implementing strict feature scaling, categorical encoding pipelines, and ensemble learning models.

---

## 🚀 Project Objectives

- **Anomalous Transaction Extraction:** Classify transaction payloads into Tiers: Legitimate (`0`) or Fraudulent (`1`).
- **Imbalanced Data Strategy:** Address severe skewness inherent to fraud classification datasets using tailored evaluation workflows.
- **Comparative Feature Valuation:** Rank spatial, temporal, and user profile properties to see what drives fraud indicators.

---

## 📊 Dataset & Schema Architecture

The pipeline processes tracking frameworks split into training and testing instances:
- `fraudTrain.csv` — Baseline parameter historical matrix used for feature tuning.
- `fraudTest.csv` — Isolated tracking framework used exclusively for model validation.

### Target Classification Labels
- **`is_fraud = 0`** 🟢 Legitimate Transaction (Majority Class)
- **`is_fraud = 1`** 🔴 Fraudulent Transaction (Minority Class)

---

## 🛠️ Tech Stack & Dependencies

- **Language Engine:** Python 3.10+
- **Data Engineering:** `pandas`, `numpy`
- **Model Training Ecosystem:** `scikit-learn`
- **Statistical Visualization:** `matplotlib`, `seaborn`

---

## ⚙️ Execution Pipeline

### 1. Data Preprocessing & Cleaning
- **Dimensionality Reduction:** Drops unstructured system identifiers (e.g., specific transaction hashes, text notes) that cause overfitting.
- **Categorical Processing:** Transforms text variables (e.g., merchant names, job roles, categories) into numeric vectors using `LabelEncoder`.
- **Feature Standardization:** normalizes highly variable numerical items (like `amt`) to zero-mean and unit-variance configurations via `StandardScaler`.

### 2. Model Pipeline Development
- Implements an ensemble **Random Forest Classifier** to create high-accuracy decision paths resilient to structural anomalies and outliers.

### 3. Model Performance Analytics
Given the highly imbalanced nature of real-world fraud distributions, performance optimization concentrates heavily on sub-class recall alongside baseline overall metrics:

| Metric Indicator | Performance Value | Insights & Focus |
| :--- | :--- | :--- |
| **Accuracy** | **99.71%** | Reflects overall correct predictions over the balanced/unbalanced system. |
| **Precision (Fraud Class)** | **0.72** | Measures fidelity—out of all flagged alerts, how many were true fraud vectors. |
| **Recall (Fraud Class)** | **0.42** | High critical threshold tracking—measures real fraud instances captured. |
| **F1-Score (Fraud Class)** | **0.53** | Harmonic mean optimizing the delicate trade-off between Precision and Recall. |

---

## 📈 Embedded Charts & Visualizations

The analytical pipeline outputs three key metric evaluation assets inside the console workbook:
1. **Confusion Matrix Plot:** Visualizes true negatives, false positives, false negatives, and true positives to audit misclassifications.
2. **Feature Importance Vector Chart:** Bar plots highlighting the top structural triggers contributing to risk probability.
3. **Accuracy Iteration Graph:** Diagnostic performance mapping metrics monitored during optimization intervals.

---

