# simple-ml-baseline-
A simple machine learning baseline project
# Machine Learning Model Comparison

## Project Overview
This project compares three machine learning algorithms using the Breast Cancer Wisconsin dataset.

## Models
1. Logistic Regression
2. Decision Tree
3. Random Forest

## Methodology
- Used the same 80/20 train-test split for all models.
- Used `random_state=42` for reproducibility.
- Evaluated using Accuracy, Precision, Recall, F1-score, and ROC-AUC.

## Results

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 0.9825 | 0.9861 | 0.9861 | 0.9861 | 0.9954 |
| Decision Tree | 0.9123 | 0.9559 | 0.9028 | 0.9286 | 0.9157 |
| Random Forest | 0.9561 | 0.9589 | 0.9722 | 0.9655 | 0.9937 |

## Conclusion
Logistic Regression achieved the highest F1-score in this experiment. Recall is also important because missing a malignant case can have serious consequences.

## How to Run
1. Install Python and Jupyter Notebook.
2. Install dependencies using `pip install -r requirements.txt`.
3. Open `baseline_model.ipynb`.
4. Run all cells from top to bottom.

## Dataset
The dataset is loaded from scikit-learn, so no separate dataset download is required.
