# MSCS_634_Lab_4

# Regression Analysis Lab – Diabetes Dataset

## Purpose

This lab explores various regression techniques to analyze and predict disease progression using the Diabetes dataset from `sklearn.datasets`. The primary goal is to understand the strengths and limitations of different regression methods, including:

- **Simple Linear Regression**
- **Multiple Linear Regression**
- **Polynomial Regression**
- **Ridge Regression**
- **Lasso Regression**

Additionally, the lab evaluates how regularization can help prevent overfitting and improve model performance.

---

## Key Insights

- **Multiple Regression** outperformed Simple Linear Regression, highlighting the benefit of incorporating multiple features.
- **Polynomial Regression** showed how increasing model complexity can lead to overfitting, especially with higher degrees (e.g., degree=10).
- **Ridge and Lasso Regression** helped control overfitting by penalizing large coefficients. Ridge retained all features, while Lasso zeroed out some, indicating feature selection.
- **BMI** was identified as a strong individual predictor of disease progression.
- The dataset is clean, preprocessed, and well-suited for regression analysis, with normalized features and no missing values.

---

## Challenges & Decisions

- Choosing the right **polynomial degree** was a key decision. Degree 2 worked well, while higher degrees caused overfitting.
- Deciding on **regularization parameters (alpha)** required experimentation. A moderate `alpha` of 1.0 for Ridge and 0.1 for Lasso provided balanced results.
- Visualization of high-dimensional models was simplified by focusing on a single feature (BMI) for polynomial regression plotting.
- Ensuring fair model comparison by using the **same train-test split** and evaluation metrics across all models.

---

## Evaluation Metrics Used

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R-squared (R² Score)

---

## Dataset

- **Source**: `sklearn.datasets.load_diabetes()`
- **Features**: 10 standardized health variables
- **Target**: Disease progression one year after baseline

---

## 📚 Tools Used

- Python (Jupyter Notebook)
- scikit-learn
- pandas, numpy
- matplotlib, seaborn

---

