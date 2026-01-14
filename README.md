# 📈 U.S. Inflation Forecasting Model

A time series forecasting system that predicts U.S. inflation trends using multiple economic indicators. This project demonstrates advanced feature engineering, model validation, and economic forecasting techniques.

![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=flat&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-success)

---

## 🎯 Project Overview

**Business Problem:** Inflation significantly impacts economic planning, investment decisions, and policy-making. Accurate inflation forecasting enables better financial planning for businesses, governments, and individuals.

**Solution:** This project builds a comprehensive forecasting pipeline that:
- Integrates multiple economic indicators as predictive features
- Applies time series decomposition and stationarity testing
- Compares multiple forecasting approaches (ARIMA, exponential smoothing, ML-based)
- Validates predictions using rolling window cross-validation

---

## 📊 Data Sources

| Indicator | Description | Source |
|-----------|-------------|--------|
| CPI | Consumer Price Index (All Items) | FRED |
| Unemployment | U.S. Unemployment Rate | BLS |
| Fed Funds Rate | Federal Funds Effective Rate | Federal Reserve |
| M2 Money Supply | M2 Money Stock | FRED |
| Oil Prices | Crude Oil Prices (WTI) | EIA |
| GDP Growth | Real GDP Growth Rate | BEA |

*Data accessed via FRED API and manual downloads*

---

## 🛠️ Methodology

### 1. Data Preprocessing
- Missing value imputation using forward-fill and interpolation
- Stationarity testing (ADF test, KPSS test)
- Seasonal decomposition (trend, seasonal, residual components)
- Feature engineering (lag features, rolling statistics, differencing)

### 2. Exploratory Data Analysis
- Correlation analysis between inflation and economic indicators
- ACF/PACF plots for lag identification
- Seasonal pattern detection

### 3. Models Implemented
| Model | Description |
|-------|-------------|
| **ARIMA** | Autoregressive Integrated Moving Average |
| **SARIMA** | Seasonal ARIMA with seasonal components |
| **Holt-Winters** | Triple exponential smoothing |
| **VAR** | Vector Autoregression (multivariate) |
| **Random Forest** | Ensemble ML approach with lag features |

### 4. Model Validation
- Train/test split with time-based ordering
- Rolling window cross-validation
- Multiple error metrics: RMSE, MAE, MAPE

---

## 📈 Key Results

| Model | RMSE | MAE | MAPE |
|-------|------|-----|------|
| ARIMA(p,d,q) | X.XX | X.XX | X.X% |
| SARIMA | X.XX | X.XX | X.X% |
| Holt-Winters | X.XX | X.XX | X.X% |
| Random Forest | X.XX | X.XX | X.X% |

*Best performing model: [Model Name] with [X]% MAPE*

---

## 📁 Repository Structure

```
Inflation_Forecast/
│
├── data/
│   ├── raw/                    # Original data files
│   └── processed/              # Cleaned datasets
│
├── notebooks/
│   ├── 01_data_collection.ipynb
│   ├── 02_eda_analysis.ipynb
│   ├── 03_feature_engineering.ipynb
│   ├── 04_modeling.ipynb
│   └── 05_evaluation.ipynb
│
├── src/
│   ├── data_loader.py          # Data ingestion functions
│   ├── preprocessing.py        # Data cleaning utilities
│   └── models.py               # Model implementations
│
├── figures/                    # Generated visualizations
├── requirements.txt
└── README.md
```

---

## 🚀 Quick Start

### Prerequisites
```bash
python >= 3.9
```

### Installation
```bash
# Clone the repository
git clone https://github.com/jfinkle00/Inflation_Forecast.git
cd Inflation_Forecast

# Install dependencies
pip install -r requirements.txt
```

### Run the Analysis
```bash
# Launch Jupyter Notebook
jupyter notebook notebooks/
```

---

## 📦 Dependencies

```
pandas>=1.4.0
numpy>=1.21.0
matplotlib>=3.5.0
seaborn>=0.11.0
statsmodels>=0.13.0
scikit-learn>=1.0.0
fredapi>=0.5.0
```

---

## 🔮 Future Improvements

- [ ] Add Prophet model for comparison
- [ ] Implement LSTM neural network approach
- [ ] Create interactive dashboard for forecast visualization
- [ ] Automate data refresh pipeline
- [ ] Add confidence intervals to predictions

---

## 👤 Author

**Jason Finkle**  
M.S. Data Science, American University

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/jason-finkle/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=flat&logo=github)](https://github.com/jfinkle00)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- Federal Reserve Economic Data (FRED) for providing accessible economic data
- American University Data Science program for foundational coursework
- Statsmodels and scikit-learn documentation and communities
