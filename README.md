# House Price Prediction — University Project

> **Original university submission.** This notebook is preserved without modifications, including its original outputs and conclusions. A subsequent review identified methodological and implementation issues involving preprocessing, cross-validation, and performance reporting. It documents an earlier stage of my learning and should not be treated as a validated predictive pipeline. Some cells require corrections before the notebook can run from beginning to end.

## Overview

This project explores house price prediction using the Kaggle House Prices dataset. It was developed as a university machine learning assignment, covering the workflow from exploratory analysis to model comparison and submission generation.

## Notebook Contents

- Exploratory data analysis: distributions, correlations, missing values, and outliers.
- Preprocessing: imputation, categorical encoding, Box-Cox transformations, and scaling.
- Feature engineering: combined measures of floor area, bathrooms, and property quality.
- Regression models: linear and regularized regression, decision trees, support vector regression, and gradient boosting.
- Feature selection with Lasso and recursive feature elimination.
- Dimensionality reduction with PCA.
- Hyperparameter search using RandomizedSearchCV and Optuna.
- Prediction averaging and generation of Kaggle submission files.

Models predict the logarithm of the sale price, with predictions converted back to the original price scale for submission.

## Known Limitations

The original workflow fits preprocessing before the internal data split and performs feature selection outside cross-validation. Some reported errors are training errors rather than out-of-sample estimates. The notebook also contains execution inconsistencies.

Its original performance claims and conclusions are retained for historical context and have not been independently revalidated.

## Data and Dependencies

The notebook expects the dataset files at:

- `house_prices/train.csv`
- `house_prices/test.csv`

The original submission-generation cells also read a template named `submission.csv`.

Main dependencies: Python, NumPy, pandas, Matplotlib, Seaborn, SciPy, scikit-learn, XGBoost, LightGBM, and Optuna.

The notebook is shared as an educational record of the original analysis, including the lessons learned from its subsequent review.
