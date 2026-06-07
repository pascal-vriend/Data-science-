# DS Project — Group 35: Atrial Fibrillation Classification

## Overview
Binary classification of atrial fibrillation (AF) from a preprocessed ECG dataset (`Preprocessed_AFData.xlsx`, 150,000 observations × 30 features + target label `Control`). The project focuses on feature engineering, dimensionality reduction, and comparing multiple classifiers.

## Pipeline

1. **Feature Engineering** — Statistical features derived from the 30 raw data columns: mean, std, variance, min, max, range, and count above mean
2. **Preprocessing** — Standard scaling + PCA (99% variance retained) to reduce dimensionality
3. **Class Imbalance** — SMOTE oversampling via `imblearn` pipeline to handle AF/No-AF imbalance
4. **Model Training & CV** — 5-fold stratified cross-validation across 7 classifiers
5. **Evaluation** — Macro recall, macro F1, classification report, and confusion matrix per model
6. **Visualisation** — Bar charts comparing macro recall and F1 across models; feature importance plots for applicable models

## Models Compared
Logistic Regression, Decision Tree, Random Forest, Linear SVM, Naive Bayes, KNN, XGBoost

## Requirements

```bash
pip install pandas numpy scikit-learn xgboost imbalanced-learn matplotlib seaborn openpyxl
```

## Usage

1. Place `Preprocessed_AFData.xlsx` in a `data/` folder
2. Open and run `Models.ipynb` top to bottom

## Repository
[github.com/pascal-vriend/Data-science-](https://github.com/pascal-vriend/Data-science-.git)
