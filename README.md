# Data Foundations

A structured, portfolio-oriented repository covering **EDA fundamentals** and a clean transition into **basic linear modeling**, plus an **applied mini-project** using a real dataset.

The emphasis is on: clear exploration, honest interpretation, and respecting the limits of what data can (and cannot) prove.

---

## Repository Structure

- `notebooks/`  
  Foundations track: EDA → relationships → linear modeling → evaluation.

- `data/`  
  Small, simple CSV files used in the foundations notebooks.

- `projects/`  
  Applied mini-projects with real datasets (each project has its own folder).

- `README_linear_models.md`  
  A focused summary of the linear modeling block (recommended reading if you want the story arc).

---

## Foundations Track (Notebooks)

### EDA Foundations
- **01_reading_tables_and_categorical_data**  
  Frequency tables + bar charts + interpretation limits for categorical data.

- **02_describing_quantitative_data**  
  Histograms, mean/median, boxplots, and how visualization changes interpretation.

- **03_comparing_groups**  
  Comparing distributions across groups (descriptive comparisons only).

- **04_variability_iqr_and_std**  
  Variability measures: IQR vs standard deviation and what each captures.

- **05_relationships_between_variables**  
  Scatter plots and cautious interpretation of association.

- **07_linear_trend_approximation**  
  A simple linear trend as an exploratory approximation tool.

- **08_eda_summary_and_limits**  
  EDA closure: what EDA helps with vs what it cannot conclude.

### Linear Modeling (Simple, Interpretable)
- **09_simple_linear_regression**  
  Fit a linear regression model (focus on meaning, not optimization).

- **10_interpreting_coefficients_and_residuals**  
  Coefficients + residual plots to assess model behavior.

- **11_when_linear_models_fail**  
  Examples of assumption violations (non-linearity, heteroscedasticity, outliers).

- **12_evaluating_linear_models**  
  Metrics (R², MAE) and why metrics don’t replace reasoning.

- **13_train_test_split_and_generalization**  
  Train/test split to evaluate generalization and avoid overly optimistic results.

➡️ For a concise narrative of the modeling block, see **`README_linear_models.md`**.

---

## Applied Projects

### Student Performance (UCI)
Location: `projects/student_performance/`

This mini-project applies the same foundations workflow to a real dataset:
- loading + first-pass cleaning
- exploratory analysis (including a discussion of potential leakage with early-period grades)
- simple modeling + evaluation
- conclusions and limitations

---

## How to Run

1. Clone the repo and move into it:
   ```bash
   git clone git@github.com:ferProg/data-foundations.git
   cd data-foundations
2. Create and activate an environment (example with venv):
    python -m venv .venv
    # Windows:
    .venv\Scripts\activate
    # macOS/Linux:
    source .venv/bin/activate
3. Install dependencies:
    pip install -U pip
    pip install pandas numpy matplotlib scikit-learn jupyter
4. Start Jupyter:
    jupyter notebook

## Notes

* Notebooks are designed to be read as a progression (not isolated exercises).

* Interpretation is intentionally cautious: association ≠ causation, and metrics ≠ truth.

* The goal is strong fundamentals and clear reasoning before advancing to more complex methods.

