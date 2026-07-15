# About the Project — House Price Prediction

## Project title
**House Price Prediction using Machine Learning**  
(Internship / Capstone style project)

## What this project is about
This project predicts the **sale price of residential houses** using property details such as quality, living area, garage size, basement area, neighborhood, and other features.

The dataset used is the **Ames Housing** dataset (similar to the Kaggle House Prices competition). The goal is to help understand **how house prices change with different features**, so pricing and property decisions can be made more confidently.

## Problem statement
1. Prepare a **complete data analysis report** on the given housing data.
2. Build a **predictive model** for house prices using available independent variables.
3. Compare multiple models and suggest the **best model for practical use**.
4. Document the **challenges faced** and the techniques used to solve them.

## Dataset
| Item | Detail |
|------|--------|
| File | `data.csv` |
| Rows | 1,460 houses |
| Columns | 81 (features + target) |
| Target | `SalePrice` — house sale price in dollars |
| Source style | Kaggle: House Prices - Advanced Regression Techniques |

Additional reference files in this repo:
- `house prices.docx` — meaning of each data field
- `PRCP-1017-AutoPricePred (4).docx` — internship task format (EDA, modeling, comparison, challenges)

> Note: The PRCP document uses a car-price example, but **this repository’s data is house prices**. The project follows the same task structure on the house-price data.

## What was done (project workflow)
1. **Exploratory Data Analysis (EDA)**  
   Checked missing values, target distribution, correlations, neighborhoods, and outliers.
2. **Data cleaning**  
   Handled missing values carefully (many “missing” values mean an amenity is absent, e.g. no pool / no alley).
3. **Feature engineering**  
   Created useful features like total square feet, total bathrooms, house age, porch area, etc.
4. **Model building**  
   Trained several regression models on a log-transformed sale price.
5. **Model comparison**  
   Compared models using RMSE, MAE, R², and RMSLE.
6. **Final recommendation**  
   Selected the best-performing model for predictions and kept a simpler model for easier business explanation.

## Models used
- Linear Regression
- Ridge / Lasso / ElasticNet
- Decision Tree
- Random Forest
- Gradient Boosting
- XGBoost

## Key findings
- Strong price drivers include **OverallQual**, **GrLivArea**, **GarageCars / GarageArea**, **TotalBsmtSF**, and **Neighborhood**.
- Sale prices are **right-skewed**, so log transformation helps modeling.
- Tree-based boosting models (especially **XGBoost**) generally performed best.

## Main deliverable
- `House_Price_Prediction_Internship.ipynb` — full internship notebook (analysis + models + comparison + challenges)  
  *(Available on the project feature branch / PR; merge if you want it on main.)*

## Tools & libraries
- Python, Jupyter Notebook
- pandas, NumPy
- Matplotlib, Seaborn
- scikit-learn, XGBoost

## How this helps (business view)
Management can use the model to:
- Estimate a fair sale price for a property
- Understand which features increase or decrease price
- Support pricing strategy with data instead of guesswork only

## Author note
Prepared as an **intern-level data science project**, with clear explanations, step-by-step analysis, and documented challenges suitable for academic / internship submission.
