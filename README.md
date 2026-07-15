# House Price Prediction (Internship Project)

Predict residential **SalePrice** from the Ames Housing dataset (`data.csv`), based on the repo materials:
- `house prices.docx` — feature dictionary / data description
- `PRCP-1017-AutoPricePred (4).docx` — internship task structure (EDA, modeling, comparison, challenges)

> Note: The PRCP brief uses a car-price example, but this repository’s dataset is **house prices**. This project applies the same internship deliverables to the house-price data provided here.

## Deliverable

Single Jupyter notebook (as required for internship submission):

**`House_Price_Prediction_Internship.ipynb`**

Contains:
1. Complete data analysis (EDA) report
2. Predictive models for `SalePrice`
3. Model comparison report + production recommendation
4. Challenges faced + techniques used

## Setup

```bash
pip install -r requirements.txt
jupyter notebook House_Price_Prediction_Internship.ipynb
```

Or run non-interactively:

```bash
jupyter nbconvert --to notebook --execute House_Price_Prediction_Internship.ipynb --output House_Price_Prediction_Internship_executed.ipynb
```

## Models compared

- Linear Regression, Ridge, Lasso, ElasticNet
- Decision Tree, Random Forest, Gradient Boosting, XGBoost

Metrics: RMSE, MAE, R², RMSLE (+ 5-fold CV on log-price).

## Dataset

- Source style: [Kaggle House Prices - Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)
- File: `data.csv` (1,460 rows × 81 columns including `SalePrice`)
