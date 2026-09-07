# House Price Prediction

Predicting residential house sale prices using the Kaggle House Prices - Advanced Regression Techniques dataset.

## Problem
Given 79 features describing the physical qualities, size, location and condition 
of houses in Ames, Iowa — predict the sale price.

## Dataset
- Source: Kaggle House Prices - Advanced Regression Techniques
- 1460 houses, 81 columns
- Target variable: SalePrice

## Results
| Model | R² | RMSE |
|---|---|---|
| Linear Regression | 0.920 | $24,738 |
| Ridge Regression | 0.919 | $25,297 |
| LASSO Regression | 0.901 | $27,574 |

## Key Findings
- Log-transforming SalePrice improved model performance by correcting right skew
- Ridge and Linear Regression performed comparably — regularisation did not 
  meaningfully improve results after feature engineering
- LASSO achieved R²=0.901 using only 79 of 260 features, demonstrating that 
  many features carry redundant information
- Recommended model: Ridge Regression

## Stack
Python, NumPy, pandas, scikit-learn, Matplotlib

## Project Structure
house_price_prediction.ipynb — full notebook with cleaning, modelling and analysis
README.md — this file