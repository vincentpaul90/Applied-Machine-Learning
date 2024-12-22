# Lasso and Ridge Regression: A Practical Comparison

This project dives into regression analysis by comparing **Lasso Regression (L1 Regularization)**, **Ridge Regression (L2 Regularization)**, and **Ordinary Least Squares (OLS)** regression. Using a real-world dataset, we explore how these methods tackle challenges like overfitting, multicollinearity, and model performance.

## Why This Project?

Linear regression is a widely used method, but it can struggle with overfitting and correlated predictors (multicollinearity). This is where **Lasso** and **Ridge** regression come in. These techniques improve model performance and interpretability by adding penalty terms that control for complexity.

## Techniques Used

### 1. **Ordinary Least Squares (OLS)**
   - **What it does**: Minimizes the sum of squared residuals to find the best-fit line.
   - **Why we used it**: To set a baseline for performance comparison.
   - **Outcome**: OLS performed well but lacked robustness when faced with overfitting or multicollinearity.

### 2. **Lasso Regression (L1 Regularization)**
   - **What it does**: Adds a penalty based on the absolute values of coefficients, shrinking some to zero (feature selection).
   - **Why we used it**: To simplify the model by eliminating irrelevant predictors.
   - **Outcome**: Lasso created a sparser model but had slightly lower accuracy compared to Ridge.

### 3. **Ridge Regression (L2 Regularization)**
   - **What it does**: Adds a penalty based on the square of coefficients, shrinking them without setting to zero.
   - **Why we used it**: To stabilize predictions and handle multicollinearity effectively.
   - **Outcome**: Ridge achieved the best balance between accuracy and stability.

## Workflow

### Step 1: Exploratory Data Analysis (EDA)
- Explored the dataset for missing values and variable relationships.
- Replaced missing values with column medians and converted categorical variables into dummy variables.

### Step 2: Data Scaling
- Standardized the data to ensure all features have comparable magnitudes.

### Step 3: Model Building
- Split the dataset into training and testing sets (70-30 split).
- Built models using OLS, Lasso, and Ridge regression.

### Step 4: Model Evaluation
- Evaluated models using:
  - **R² Score**: Measures the proportion of variance explained by the model.
  - **Root Mean Squared Error (RMSE)**: Indicates average prediction error.
- Performed residual analysis to check the goodness of fit.

### Step 5: Visualization
- Plotted residuals and compared actual vs. predicted values to visually analyze model performance.

## Results

| Metric                       | OLS          | Lasso (α=0.1)  | Ridge (α=0.3) |
|------------------------------|--------------|----------------|---------------|
| **Training R² Score**        | 0.836        | 0.799          | 0.836         |
| **Test R² Score**            | 0.844        | 0.810          | 0.844         |
| **Root Mean Squared Error**  | 0.37         | 0.40           | 0.37          |

### Key Insights:
- **OLS**: Strong baseline but lacks regularization, making it prone to overfitting.
- **Lasso**: Simplifies the model by reducing some coefficients to zero but sacrifices some accuracy.
- **Ridge**: Offers the best trade-off between accuracy and robustness.



