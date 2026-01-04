# 📈 sales-demand-forecasting-tsa

### Sales Demand Forecasting & Economic Driver Analysis using Time Series Analysis

## 📌 Project Overview
This project focuses on forecasting future sales demand using historical time series data combined with key economic exogenous variables. By integrating financial and cost-related drivers into a statistical forecasting model, the project delivers accurate, interpretable, and business-relevant predictions.

## 🎯 Objective
To build a high-precision predictive model that forecasts future sales quantities based on historical trends and key economic exogenous variables, enabling data-driven inventory and financial planning.

## 🧾 Dataset Description
- File Name: Month_Value_1.csv  
- Frequency: Monthly  
- Target Variable: Sales Quantity  
- Exogenous Variables:
  - Revenue
  - Average Cost
  - Regional Payroll

## 🔍 Methodology

### Data Preprocessing
- Cleaned the dataset and converted periods to a DateTime index
- Applied linear interpolation to ensure a continuous time series

### Stationarity Diagnostics
- Applied the Augmented Dickey-Fuller (ADF) test
- Raw series was non-stationary (p = 0.55)
- First-order differencing achieved stationarity (p ≈ 0)

### Exogenous Variable Integration
- Incorporated Revenue, Average Cost, and Regional Payroll as external drivers

### Model Development
- Model Used: SARIMAX (Seasonal ARIMA with Exogenous Variables)
- Configuration: SARIMAX(1, 1, 1)
- Train-Test Split: 80% / 20%

### Model Evaluation
- Evaluation Metric: Mean Absolute Error (MAE)
- MAE = 157.35, indicating high accuracy relative to sales scale

## 📊 Forecasting & Results

### Strategic Forecasting
- Forecasted 24 months of future sales
- Assumed a 1% monthly revenue growth rate

### Forecast Insights
- Predicts a steady upward trend in sales demand
- Sales volume is expected to reach approximately 32,000 units by 2024, assuming consistent revenue growth

## 🔑 Key Findings
- Revenue and Average Cost are the most significant predictors of sales demand 
- Regional Payroll shows comparatively lower influence

## 💼 Business Impact
This project provides a reliable forecasting framework for inventory management and financial planning, enabling businesses to anticipate demand based on financial targets rather than intuition.

## 🛠️ Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Statsmodels
- pmdarima
- Jupyter Notebook

## 📁 Repository Structure
data/        → Raw and cleaned datasets  
notebooks/  → Step-by-step analysis and modeling  
results/    → Forecast outputs and visualizations  
report/     → Final project report (PDF)

## 📌 Conclusion
The sales-demand-forecasting-tsa project demonstrates how time series forecasting combined with economic exogenous variables can deliver accurate and interpretable sales predictions, supporting real-world business decision-making.

## 📊 Dataset
The dataset used in this project is sourced from **Kaggle**. 
You can find the original data here: [https://www.kaggle.com/datasets/podsyp/time-series-starter-dataset]

*Note: The dataset contains monthly business records including sales quantity, revenue, and cost metrics.*


