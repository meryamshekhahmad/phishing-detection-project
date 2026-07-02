# Phishing Detection Final Project

Course: **Data Science in Cybersecurity**

## Project Description

This repository contains a clean final project that critically reproduces and evaluates the paper **"Phishing Detection Using Machine Learning Techniques"**. The project trains and evaluates machine-learning models for phishing website detection using engineered URL, HTML, domain, and reputation features.

The notebook includes data loading, inspection, EDA, feature engineering, model training, evaluation, error analysis, and reproducibility analysis.

The updated version also includes deployment-focused experiments requested after review:

- PR-AUC / Average Precision
- F2-score
- Precision-Recall curves
- Threshold tuning
- Error trade-off analysis for false positives and false negatives

## Selected Paper

**Phishing Detection Using Machine Learning Techniques**  
Authors: Vahid Shahrivari, Mohammad Mahdi Darabi, Mohammad Izadi

## Original GitHub Repository

https://github.com/fafal-abnir/phishing_detection

## Dataset Source

The dataset is copied from the original GitHub repository and stored locally in:

```text
data/dataset.csv
```

Original labels:

- `-1` = phishing
- `1` = legitimate

The notebook encodes phishing as the positive class for evaluation.

## Python Version

Tested with **Python 3.12**.

## Dependencies

Required packages are listed in `requirements.txt`:

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
jupyter
```

## Installation Instructions

Create and activate a fresh Python environment, then install dependencies:

```bash
pip install -r requirements.txt
```

## How to Run the Notebook

From the project root, run:

```bash
jupyter notebook final_project_phishing_detection.ipynb
```

Then run all cells from top to bottom.

## Folder Structure

```text
.
├── final_project_phishing_detection.ipynb
├── report.md
├── report.pdf
├── README.md
├── requirements.txt
└── data/
    └── dataset.csv
```

## Main Project Sections

- Data loading from `data/dataset.csv`
- Data inspection and quality checks
- Class imbalance analysis
- Feature distributions and outlier analysis
- Spearman correlation analysis
- Feature engineering and preprocessing
- Stratified train/test split with `random_state=42`
- Logistic Regression, Decision Tree, Random Forest, and XGBoost
- Accuracy, Precision, Recall, F1, MCC, ROC-AUC, and confusion matrix
- PR-AUC / Average Precision and F2-score
- Precision-Recall curves
- Cybersecurity-aware threshold tuning
- False positive and false negative error analysis
- Reproducibility analysis
