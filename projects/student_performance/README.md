⬅️ Back to repository overview: [README.md](../../README.md)  
➡️ Linear models foundations: [README_linear_models.md](../../README_linear_models.md)

# Student Performance (UCI) — Applied Mini Project

This project applies the foundations workflow (EDA → modeling → evaluation) to a real-world educational dataset.
The emphasis is on **clear reasoning**, **reproducibility**, and **honest interpretation**, not on optimization or leaderboard performance.

---

## Goal

Explore factors associated with student performance and build simple, interpretable models to predict the final grade (**G3**), while explicitly discussing limitations and potential information leakage.

---

## Dataset

Source: UCI Machine Learning Repository — *Student Performance*  
File(s) used:
- `data/student-mat.csv` (raw)
- `data/student-mat-clean.csv` (cleaned output produced in Notebook 01)

The UCI CSV uses `;` as a separator.

---

## Project Structure

- `data/`
  - raw and cleaned datasets used throughout the project

- `notebooks/`
  - sequential notebooks documenting the full workflow

---

## Notebooks

### 01 — Loading and cleaning
- [01_loading_and_cleaning.ipynb](notebooks/01_loading_and_cleaning.ipynb)

- Load the raw dataset
- Initial data quality checks (types, missing values, duplicates)
- First-pass cleaning
- Export cleaned dataset for consistent downstream use

### 02 — Exploratory analysis
- [02_exploratory_analysis.ipynb](notebooks/02_exploratory_analysis.ipynb)

- Target distribution (G3)
- Key relationships and group comparisons
- Hypotheses to guide modeling
- Explicit discussion of modeling scenarios

### 03 — Simple modeling 
- [03_simple_modeling.ipynb](notebooks/03_simple_modeling.ipynb)

- Train/test split
- Baseline linear model
- Model comparison with and without early-period grades

### 04 — Conclusions and limits
- [04_conclusions_and_limits.ipynb](notebooks/04_conclusions_and_limits.ipynb)

- Summary of findings
- Practical interpretation and limits
- What this analysis cannot conclude
- Next steps and improvements

---

## Target and Leakage Note (G1/G2)

- Primary target: **G3** (final grade)
- **G1** and **G2** are grades from earlier periods and can be highly predictive.

Depending on the use-case, using G1/G2 may be:
- **Valid** (late-stage prediction, when earlier grades are available), or
- **Information leakage** (early-stage prediction, when those grades are not yet known)

For this reason, models will be evaluated **both with and without G1/G2**.

---

## Evaluation Approach

Evaluation will prioritize generalization over in-sample fit:
- Train/test split
- Metrics such as MAE and R² interpreted cautiously
- Residual checks for model assumptions (where relevant)

---

## Next Steps

- Build baseline models (with vs. without G1/G2)
- Compare performance and interpretability
- Document conclusions and limitations clearly
- Consider extending to multiple regression and stronger diagnostics
