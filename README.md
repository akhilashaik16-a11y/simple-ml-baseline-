# Task 03 — Features and Tuning

## Overview
This project uses the Breast Cancer Wisconsin dataset to demonstrate feature engineering, cross-validation, and hyperparameter tuning.

## What is included
- Three engineered features: `radius_area_proxy`, `texture_smoothness_interaction`, and `worst_to_mean_radius_ratio`
- Stratified 5-fold cross-validation
- `GridSearchCV` for Logistic Regression hyperparameters
- Before-and-after test metrics: accuracy, malignant-class precision, malignant-class recall, malignant-class F1, and ROC-AUC

## Run in Google Colab
1. Open https://colab.research.google.com/
2. Upload `improved_model.ipynb`.
3. Select **Runtime → Run all**.
4. Review the best parameters and the before-and-after comparison table.

## Run locally
Install dependencies, then open the notebook in Jupyter:
```bash
pip install -r requirements.txt
jupyter notebook improved_model.ipynb
```

## Evaluation decisions
- A stratified 80/20 train/test split is used.
- Cross-validation and tuning run only on the training set.
- The test set is held out for the final comparison.
- Malignant (class label 0 in scikit-learn's dataset) is explicitly treated as the positive class for precision, recall, and F1 in the final comparison.
- Improvements are measured, not assumed; scores can vary with library versions.
