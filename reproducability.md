# Predicting Term Deposit Subscriptions: A Complete Machine Learning Pipeline

Authors:
- Lydia Brorsson
- Francesco Dorati

## Overview

This project builds and evaluates a complete machine learning pipeline for predicting whether a bank client will subscribe to a term deposit product using the UCI Bank Marketing dataset.

The project includes:

- Exploratory Data Analysis (EDA)
- Data preprocessing
- PCA and clustering (K-Means, GMM)
- Logistic Regression, Ridge and Lasso
- Support Vector Machines
- Random Forest and Gradient Boosting
- Model comparison and selection

## Requirements
This project was developed and tested using:

- Python 3.10.13

Install dependencies using:

pip install -r requirements.txt

## Running the Project

1. Place the dataset file in the same directory as the notebook.
2. Open `ml_project.ipynb`.
3. Run all cells from top to bottom.

The notebook will automatically:

- preprocess the data
- generate all figures
- train and evaluate all models
- reproduce the results reported in the paper

## Reproducibility

All experiments use a fixed random seed:

random_state = 42

This ensures reproducible train-test splits, cross-validation folds, and model training procedures.

## Expected Results

Approximate cross-validated ROC-AUC scores:

- Logistic Regression: 0.881
- SVM (RBF): 0.900
- Random Forest: 0.922
- Gradient Boosting: 0.924

Expected test ROC-AUC for the final Gradient Boosting model:

0.922

## Notes

The project was developed using Python and scikit-learn.

Some figures may take a few minutes to generate depending on hardware, particularly during SVM hyperparameter tuning.