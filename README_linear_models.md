# Linear Models — Exploratory Analysis and Simple Regression

This block covers the fundamentals of exploratory data analysis (EDA) and simple linear regression, with a focus on **understanding**, not optimization.

The goal is to learn how data behaves, what linear models can and cannot explain, and how interpretation changes depending on the analytical lens.

---

## 📊 Notebooks Overview

### 01 — Reading Tables and Categorical Data
- Loading simple CSV files
- Frequency tables
- Bar charts
- What can be observed vs. what cannot be concluded

### 02 — Describing Quantitative Data
- Histograms
- Mean and median
- Boxplots
- How visualization affects interpretation

### 03 — Comparing Groups
- Grouped summaries
- Visual comparison
- Limitations of group-based inference

### 04 — Variability: IQR and Standard Deviation
- Measures of spread
- Robust vs. non-robust statistics
- When variability matters more than central tendency

### 05 — Relationships Between Variables
- Scatter plots
- Direction, form, and strength
- Correlation vs. explanation

### 07 — Linear Trend Approximation
- Visual trend estimation
- Line as a descriptive tool
- Avoiding premature modeling

### 08 — EDA Summary and Limits
- What EDA can answer
- What EDA cannot answer
- Why modeling decisions should not be rushed

---

## 📈 Linear Regression Block

[## 09_simple_linear_regression](notebooks/09_simple_linear_regression.ipynb)
- Fitting a basic linear model
- Interpreting slope and intercept
- Linear relationship assumptions

[## 10_interpreting_coefficients_and_residuals](notebooks/10_interpreting_coefficients_and_residuals.ipynb)
- Meaning of coefficients
- Residual analysis
- What residuals reveal about model fit

[## 11_when_linear_models_fail](notebooks/11_when_linear_models_fail.ipynb)
- Non-linearity
- Heteroscedasticity
- Outliers and leverage points

[## 12_evaluating_linear_models](notebooks/12_evaluating_linear_models.ipynb)
- R², MAE, and their interpretation
- Why metrics alone are not enough
- The danger of metric-driven conclusions

[## 13_train_test_split_and_generalization](notebooks/13_train_test_split_and_generalization.ipynb)
- Separating training and testing data
- Evaluating performance on unseen data
- Overfitting and generalization limits

---

## 🧠 Key Principles Emphasized

- Visualization precedes modeling
- Metrics do not replace reasoning
- Linear models are explanatory tools, not universal solutions
- Simplicity and interpretability are prioritized over performance

---

## ⚠️ Limitations

- Only simple linear relationships are explored
- No hyperparameter tuning or model optimization
- No multivariate or non-linear models

These limitations are intentional and aligned with the educational goal of this block.

---

## 🔜 Next Steps

Future work may include:
- Model diagnostics and assumptions
- Multiple linear regression
- Non-linear models
- Applied mini-projects with real-world datasets

⬅️ Back to repository overview: [README.md](README.md)

