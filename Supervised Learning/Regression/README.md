# Regression Model Comparison

This project demonstrates a detailed comparison of various regression models, including **Linear Regression**, **Ridge Regression**, and **Lasso Regression**. The goal is to understand the strengths and weaknesses of each model by evaluating their performance on a given dataset.

## Overview

In this project:
- Implemented and compared three regression models: Linear Regression, Ridge Regression, and Lasso Regression.
- Evaluated the models using metrics such as **R² Score** and **Root Mean Squared Error (RMSE)**.
- Visualized the results using **Matplotlib** and **Seaborn** for insights into model performance and residuals.

## Key Results

| Model                | R² Score (Test Data) | RMSE (Test Data) |
|----------------------|----------------------|------------------|
| Linear Regression    | 0.84                | 0.37             |
| Ridge Regression     | 0.85                | 0.35             |
| Lasso Regression     | 0.80                | 0.40             |

### Insights
- **Linear Regression**: Provides a good baseline but may overfit in some cases.
- **Ridge Regression**: Performs best due to regularization, which prevents overfitting by shrinking coefficients.
- **Lasso Regression**: Simplifies the model by reducing some coefficients to zero, making it ideal for feature selection.

## Skills and Tools

This project highlights the following skills and tools:
- **Programming Language**: Python
- **Libraries**:
  - `scikit-learn` for implementing regression models.
  - `Matplotlib` and `Seaborn` for visualizations.
  - `Pandas` and `NumPy` for data manipulation.
- **Regression Techniques**:
  - Ordinary Least Squares (OLS)
  - L1 Regularization (Lasso)
  - L2 Regularization (Ridge)

