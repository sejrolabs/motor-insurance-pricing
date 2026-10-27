# Motor Insurance Pricing

**Actuarial modeling, statistical learning and interactive pricing simulation**

## Overview

This project develops an actuarial pricing framework for motor insurance using frequency-severity modeling. It compares classical Generalized Linear Models (GLMs) with machine learning approaches to estimate expected claim costs and analyze the main risk factors.

## Objectives

- Model claim frequency and average claim severity.
- Estimate pure premiums at the policy level.
- Compare actuarial models with machine learning alternatives.
- Evaluate predictive performance, calibration and interpretability.
- Build an interactive Streamlit application.

## Data

The project uses the `freMTPL2freq` and `freMTPL2sev` datasets from CASdatasets.

See [`data/README.md`](data/README.md) for data provenance, access instructions, variable definitions and preprocessing conventions.

## Methodology

1. Exploratory data analysis and data quality checks.
2. Poisson and, where appropriate, negative binomial frequency models.
3. Gamma severity modeling.
4. Random Forest and XGBoost comparisons.
5. Pure premium estimation and model calibration.
6. SHAP-based interpretation and sensitivity analysis.

## Evaluation

The analysis considers frequency and severity deviance, aggregate cost prediction, calibration by risk decile and model interpretability.

**Results will be reported here after the experiments have been run and validated.**

## Application

The Streamlit application allows users to explore risk profiles, compare predictions and inspect the estimated pure premium.

## Installation

```bash
git clone https://github.com/YOUR-PSEUDO/motor-insurance-pricing.git
cd motor-insurance-pricing
python -m venv .venv
pip install -r requirements.txt
```

Activate the virtual environment before installing dependencies. See the setup instructions for your operating system.

## Project structure

- `notebooks/`: exploration and experiments
- `src/`: reusable modeling code
- `tests/`: automated tests
- `app/`: interactive application
- `reports/`: results and visualizations
- `docs/`: methodology, assumptions and limitations

## Limitations

The pure premium is an expected claim cost, not a complete commercial premium. Expenses, taxes, commissions, profit margins and underwriting constraints are outside the baseline scope.

## Authors

Toussaint B., Fathnelle M.

## License

See [`LICENSE`](LICENSE).

