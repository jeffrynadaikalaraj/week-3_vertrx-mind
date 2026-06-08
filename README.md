# week-3_vertrx-mind

# 🩺 Breast Cancer Prediction - Model Evaluation & Hyperparameter Tuning

## 📌 Project Overview

This project focuses on building and evaluating a Machine Learning model for Breast Cancer Prediction using the Scikit-Learn Breast Cancer Dataset.

The objective is to evaluate model performance using advanced classification metrics and improve the model through hyperparameter tuning.

---

## 🎯 Objectives

- Train a classification model
- Calculate Precision, Recall, and F1-Score
- Generate a Confusion Matrix
- Perform Hyperparameter Tuning using GridSearchCV
- Compare model performance before and after tuning

---

## 🛠 Technologies Used

- Python
- Pandas
- Matplotlib
- Scikit-Learn
- Jupyter Notebook

---

## 📊 Dataset

Dataset Source:

```python
from sklearn.datasets import load_breast_cancer
```

The Breast Cancer Wisconsin Dataset is a built-in dataset provided by Scikit-Learn.

### Dataset Information

- Samples: 569
- Features: 30
- Classes:
  - 0 → Malignant
  - 1 → Benign

---

## 🚀 Project Workflow

### Step 1: Data Loading

Load the Breast Cancer dataset from Scikit-Learn.

### Step 2: Train-Test Split

Split data into:

- 80% Training Data
- 20% Testing Data

### Step 3: Model Training

Train a Random Forest Classifier.

### Step 4: Metrics Evaluation

Calculate:

- Precision
- Recall
- F1 Score

### Step 5: Confusion Matrix

Visualize model predictions using a confusion matrix.

### Step 6: Hyperparameter Tuning

Use GridSearchCV with 5-Fold Cross Validation to find the best model parameters.

### Step 7: Final Evaluation

Evaluate the tuned model and compare performance with the baseline model.

---

## 📈 Results

Confusion Matrix:

| Actual / Predicted | 0 | 1 |
|-------------------|---|---|
| 0 | 40 | 3 |
| 1 | 1 | 70 |

### Performance Metrics

| Metric | Score |
|----------|---------|
| Accuracy | 96.49% |
| Precision | 95.89% |
| Recall | 98.59% |
| F1 Score | 97.22% |

---

## 🔍 Hyperparameter Tuning

GridSearchCV was used with:

```python
param_grid = {
    "n_estimators": [50, 100, 200],
    "max_depth": [5, 10, None]
}
```

Cross Validation:

- 5-Fold CV
- Scoring Metric: F1 Score

---

## 📂 Project Structure

```text
Breast-Cancer-Prediction/
│
├── Breast_Cancer_Prediction.ipynb
├── README.md
└── requirements.txt
```

---

## ▶️ How to Run

Clone the repository:

```bash
git clone <your-repository-url>
```

Install dependencies:

```bash
pip install pandas matplotlib scikit-learn
```

Run the notebook:

```bash
jupyter notebook
```

Open:

```text
Breast_Cancer_Prediction.ipynb
```

---

## 📚 Learning Outcomes

Through this project, the following concepts were applied:

- Classification Algorithms
- Model Evaluation Metrics
- Confusion Matrix Analysis
- Hyperparameter Tuning
- Cross Validation
- Machine Learning Workflow

---

## 👨‍💻 Author

Developed as part of a Machine Learning Model Evaluation & Tuning project using Scikit-Learn.
