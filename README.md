# 📈 Inflation Forecasting Project

## Overview
This project focuses on building predictive models to forecast **inflation rates** using a combination of macroeconomic indicators and machine learning techniques.

## Project Goals
- Analyze historical inflation data
- Identify key economic indicators correlated with inflation
- Build and evaluate forecasting models
- Visualize trends and model predictions

## Data Sources
- Inflation rate data (e.g., CPI)
- Economic indicators (e.g., PPI, wages, commodity prices)

## Techniques Used
- Exploratory Data Analysis (EDA) with pandas and matplotlib
- Machine Learning models (e.g., Random Forest, XGBoost)
- Time Series Forecasting (e.g., ARIMA)
- Model Evaluation Metrics (RMSE, MAE, AIC)

## File Structure
- `inflationFC.ipynb`: Main notebook containing data processing, modeling, and visualization steps.

## How to Run
```bash
pip install pandas numpy matplotlib scikit-learn statsmodels xgboost
jupyter notebook inflationFC.ipynb
```
Follow the notebook cells sequentially for data loading, preprocessing, modeling, and evaluation.

## Exploratory Data Analysis
<img width="1005" height="547" alt="image" src="https://github.com/user-attachments/assets/5387d159-fa70-41d8-adea-4226665fb9a5" />
<img width="1005" height="547" alt="image" src="https://github.com/user-attachments/assets/2f617f93-8fed-45c6-b6dd-723819ec8751" />
<img width="996" height="547" alt="image" src="https://github.com/user-attachments/assets/f64a63d7-fbbb-424c-bf4e-29d03bbd68ed" />
<img width="1023" height="547" alt="image" src="https://github.com/user-attachments/assets/43621c5a-3ffa-4fb6-ba56-623000d33ee4" />
<img width="996" height="547" alt="image" src="https://github.com/user-attachments/assets/536b1b8c-1ac1-4db5-8552-4137c90fb269" />




## Results Summary
<img width="1390" height="590" alt="image" src="https://github.com/user-attachments/assets/7e999d4f-625c-485b-ab82-0cf744601cc3" />
<img width="1163" height="624" alt="image" src="https://github.com/user-attachments/assets/ba1e9c70-8d96-466b-8998-d2fdf9fffe61" />


LSTM Predictions

Date	
2024-07-01	315.009766

2024-08-01	315.674164

2024-09-01	316.276123

2024-10-01	316.854980

2024-11-01	317.437714

2024-12-01	318.047913

2025-01-01	318.720490

2025-02-01	319.498657

2025-03-01	320.324951

2025-04-01	321.093628

2025-05-01	321.835297

2025-06-01	322.521759


## Future Improvements
- Incorporate more advanced time series models (e.g., LSTM)
- Hyperparameter tuning with cross-validation
- Deployment of the model via a dashboard

## Author
Created by Jason Finkle. Open for collaboration and feedback!
