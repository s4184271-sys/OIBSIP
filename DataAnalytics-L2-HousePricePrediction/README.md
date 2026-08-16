# House Price Prediction

**Track:** Data Analytics (Level 2, Task 1)
**Author:** Syed Mohammed Ghouse

## Objective
Build and evaluate a linear regression model that predicts house prices based on features such as size, quality, garage capacity, and age.

## Dataset
Source: [Ames Housing Dataset — Kaggle](https://www.kaggle.com/datasets/shashanknecrothapa/ames-housing-dataset)
- 2,930 houses, 82 features, target variable: `SalePrice`

## What This Notebook Covers
1. **EDA** — structure, data types, missing value analysis
2. **Missing Value Handling** — context-aware fill strategy (None / 0 / median depending on what "missing" means for each column)
3. **Feature Selection** — 10 features chosen based on correlation with price
4. **Correlation Analysis** — heatmap + multicollinearity check
5. **Model Training** — Linear Regression with 80/20 train/test split
6. **Evaluation** — MAE, RMSE, R², actual vs predicted scatter plot, residual plot
7. **Coefficient Analysis** — interpreting what drives price
8. **Bonus: One-Hot Encoding** — added `Neighborhood` as a categorical feature, improving R² from 0.80 to 0.84

## Key Results
- **R² Score: 0.80** (0.84 with neighborhood data included)
- **MAE: $24,856**
- **RMSE: $39,562**
- Strongest predictor: `Overall Qual` (~$19,547 per quality point)
- Model underpredicts high-value homes (>$400K), likely due to unmodeled premium features

## Tools Used
Python, pandas, matplotlib, seaborn, scikit-learn, Jupyter Notebook

## Files
- `House_Price_Prediction.ipynb` — full analysis notebook
- `AmesHousing.csv` — dataset
