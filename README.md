# Ridge Regression Analysis

This project explores multicollinearity and regularized regression using the Real Estate Valuation dataset. It compares Ordinary Least Squares (OLS) methods with Ridge Regression and evaluates how regularization improves stability when predictor variables are highly correlated.

## Overview

The analysis covers:

- data cleaning and preprocessing
- descriptive statistics and distribution checks
- feature relationships and correlation analysis
- multicollinearity diagnostics using condition numbers and variance inflation factors (VIF)
- OLS estimation using:
  - normal equations
  - QR decomposition
  - singular value decomposition (SVD)
- Ridge Regression implementation and ridge trace analysis
- model selection using k-fold cross-validation

## Dataset

The project uses the Real Estate Valuation dataset from the UCI Machine Learning Repository.

Files in the repository:

- `data/raw/real_estate_data.csv`
- `data/processed/real_estate_data_updated.csv`

## Project Structure

```text
Ridge/
├── README.md
├── .gitignore
├── requirement.txt
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   ├── data_processing/
│   └── implementation/
├── results/
├── notebooks.zip
├── results.zip
└── .git/
```

## Environment Setup

Create a Python environment and install dependencies:

```bash
python -m venv .venv
source .venv/bin/activate    # macOS / Linux
# or .venv\Scripts\activate  # Windows
pip install -r requirement.txt
```

## Running the Analysis

Open the notebooks in order under `notebooks/`:

1. `notebooks/data_processing/01_test.ipynb`
2. `notebooks/data_processing/02_updated_csv.ipynb`
3. `notebooks/data_processing/03_descriptive_statistics.ipynb`
4. `notebooks/data_processing/04_distribution_analysis.ipynb`
5. `notebooks/data_processing/05_outlier_analysis.ipynb`
6. `notebooks/data_processing/06_feature_relationships.ipynb`
7. `notebooks/data_processing/07_correlation_analysis.ipynb`
8. `notebooks/data_processing/08_multicollinearity.ipynb`
9. `notebooks/implementation/09_ols_normal_equations.ipynb`
10. `notebooks/implementation/10_ols_qr_decomposition.ipynb`
11. `notebooks/implementation/11_ols_svd.ipynb`
12. `notebooks/implementation/12_ols_comparisons.ipynb`
13. `notebooks/implementation/13_ridge_regression.ipynb`
14. `notebooks/implementation/14_ridge_trace_analysis.ipynb`
15. `notebooks/implementation/15_ridge_kfold_cross_validation.ipynb`

## Dependencies

The project uses:

- NumPy
- Pandas
- Matplotlib
- Seaborn
- SciPy
- Scikit-learn
- Statsmodels
- Jupyter Notebook
- ucimlrepo

## Contributors

- Nitisha Choudhary
- Mukesh Kumar
- Adyasha Parida
- Rohit Nandha

## Project Status

Most of the core analysis notebooks are present and structured in sequence, including data processing, OLS comparison, Ridge Regression, ridge trace, and cross-validation analysis.

## Notes

- The repository currently contains analysis notebooks rather than a packaged Python module.
- The dependency file is named `requirement.txt` (singular), so install with `pip install -r requirement.txt`.
- Generated outputs and archived project bundles are stored in `results/` and zip files in the root directory.
