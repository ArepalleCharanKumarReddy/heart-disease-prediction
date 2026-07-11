# ❤️ Heart Disease Prediction using Machine Learning

> An end-to-end supervised machine learning pipeline for heart disease prediction using comprehensive exploratory data analysis (EDA), robust data preprocessing, feature scaling, class imbalance handling with SMOTE, hyperparameter optimization, and comparative evaluation of multiple machine learning models.

---

## 📌 Project Overview

Cardiovascular diseases remain one of the leading causes of mortality worldwide, making early diagnosis an important healthcare challenge. This project develops an end-to-end machine learning framework to predict the presence of heart disease using clinical and physiological attributes collected from the UCI Heart Disease dataset.

Unlike implementations that focus only on model training, this project emphasizes the complete machine learning lifecycle, including data exploration, preprocessing, feature preparation, model development, hyperparameter optimization, and comprehensive performance evaluation.

Four supervised machine learning algorithms were implemented and compared to identify the most effective model for binary heart disease prediction.

---

## ✨ Key Features

- Comprehensive Exploratory Data Analysis (EDA)
- Missing value analysis and imputation
- Numerical and categorical feature handling
- Outlier detection and removal using the IQR method
- Feature scaling using Min-Max Scaling and Standardization
- Class imbalance handling using SMOTE
- Hyperparameter optimization using RandomizedSearchCV
- Comparative evaluation of multiple machine learning models
- Performance analysis using:
  - Accuracy
  - Precision
  - Recall
  - F1 Score
  - Confusion Matrix
  - ROC Curve
  - Precision-Recall Curve
- Well-documented Jupyter Notebook with step-by-step implementation

---

## 📂 Repository Structure

```text
heart-disease-prediction/
│
├── dataset/
│   └── heart_disease_uci.csv
│
├── notebooks/
│   └── heart_disease_prediction.ipynb
│
├── presentation/
│   └── HeartDiseasePredictionPresentation.pdf
│
├── README.md
└── requirements.txt
```

---

## 📊 Dataset

This project utilizes the **Heart Disease UCI Dataset**, a widely used benchmark dataset for binary and multiclass heart disease prediction research.

### Dataset Summary

| Property | Value |
|----------|-------|
| Source | UCI Machine Learning Repository |
| Records | 920 |
| Features | 16 |
| Prediction Task | Binary Classification |
| Target Variable | `num` |

The original target variable contains five classes:

| Value | Meaning |
|-------|---------|
| 0 | No Heart Disease |
| 1–4 | Presence of Heart Disease (increasing severity) |

For this project, the target variable was transformed into a **binary classification problem**:

| Binary Value | Meaning |
|-------------|---------|
| 0 | No Heart Disease |
| 1 | Heart Disease Present |

---

## 🛠️ Technology Stack

### Programming Language

- Python

### Development Environment

- Jupyter Notebook

### Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)
- XGBoost
- LightGBM

---

## 🔄 Project Workflow

The project follows a structured machine learning pipeline from raw clinical data to model evaluation.

```text
Environment Setup
        │
        ▼
Dataset Loading
        │
        ▼
Exploratory Data Analysis (EDA)
        │
        ▼
Data Preprocessing
        │
        ▼
Post-Cleaning Analysis
        │
        ▼
Train-Test Split
        │
        ▼
Feature Scaling
        │
        ▼
SMOTE for Class Balancing
        │
        ▼
Model Training
        │
        ▼
Model Evaluation
        │
        ▼
Performance Comparison
```

---

## ⚙️ Machine Learning Pipeline

### 1. Exploratory Data Analysis

The dataset was explored to understand its characteristics before model development.

Performed analyses include:

- Dataset structure inspection
- Feature identification
- Statistical summaries
- Missing value analysis
- Target class distribution
- Histogram analysis
- Boxplot analysis
- Outlier detection

---

### 2. Data Preprocessing

The preprocessing pipeline includes:

- Binary target conversion
- Missing value imputation
- Median imputation for numerical features
- Mode imputation for categorical features
- Outlier removal using the Interquartile Range (IQR) method
- Feature scaling
- Data preparation for model training

---

### 3. Class Imbalance Handling

To improve model learning, class imbalance was addressed using the **Synthetic Minority Oversampling Technique (SMOTE)**.

SMOTE was applied **only to the training dataset**, preventing information leakage into the testing data.

---

### 4. Model Development

Four supervised machine learning algorithms were implemented and evaluated.

| Model |
|--------|
| Support Vector Machine (SVM) |
| Random Forest |
| XGBoost |
| LightGBM |

Hyperparameter optimization was performed using **RandomizedSearchCV** where applicable to improve predictive performance.

---

## 📈 Model Performance

Four supervised machine learning models were trained and evaluated for binary heart disease prediction.

| Model | Accuracy |
|--------|----------|
| Support Vector Machine (SVM) | **86.96%** |
| Random Forest | **86.96%** |
| LightGBM | **88.59%** |
| XGBoost | **90.22%** |

### Best Performing Model

**XGBoost** achieved the highest overall predictive performance among the evaluated models, providing the best balance between classification accuracy and generalization.

---

## 📊 Evaluation Metrics

The models were evaluated using multiple performance metrics rather than relying solely on accuracy.

Evaluation metrics include:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Receiver Operating Characteristic (ROC) Curve
- Area Under the ROC Curve (AUC)
- Precision–Recall Curve

This comprehensive evaluation provides a more reliable assessment of model performance, particularly for medical classification tasks.

---

## 🚀 Getting Started

### Clone the Repository

```bash
git clone https://github.com/ArepalleCharanKumarReddy/heart-disease-prediction.git
```



---

### Navigate to the Project Directory

```bash
cd heart-disease-prediction
```

---

### Install Required Dependencies

```bash
pip install -r requirements.txt
```

---

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```
notebooks/heart_disease_prediction.ipynb
```

and execute the notebook cells sequentially.

---

## 📁 Project Documentation

The repository contains the following project resources:

| Resource | Description |
|----------|-------------|
| `notebooks/` | Complete implementation of the machine learning pipeline |
| `dataset/` | UCI Heart Disease dataset used for training and evaluation |
| `presentation/` | Detailed project presentation covering methodology, experimental results, and conclusions |

The presentation provides a detailed explanation of:

- Project motivation
- Dataset overview
- Exploratory Data Analysis
- Data preprocessing
- Machine learning pipeline
- Model comparison
- Performance evaluation
- Final conclusions

---

## 🎯 Future Improvements

Potential future enhancements include:

- Deep Learning–based prediction models
- Explainable AI (SHAP / LIME)
- Feature selection techniques
- Cross-validation-based evaluation
- Model deployment using Flask or FastAPI
- Interactive web application for prediction
- Real-time clinical decision support interface

---

## 👨‍💻 Author

**Arepalle Charan Kumar Reddy**

B.Tech – Artificial Intelligence and Machine Learning

Amrita Vishwa Vidyapeetham

---

## 🙏 Acknowledgements

- UCI Machine Learning Repository
- Scikit-learn
- XGBoost
- LightGBM
- Imbalanced-learn

---

## ⭐ If you found this repository useful

If this project helped you understand the machine learning pipeline for heart disease prediction, consider giving the repository a ⭐ on GitHub.
