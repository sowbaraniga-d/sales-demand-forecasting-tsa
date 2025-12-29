# sales-demand-forecasting-tsa
Time series analysis and forecasting of monthly sales data using statistical modeling to predict future demand trends.
This project focuses on identifying long-term patterns in sales data and building a robust predictive model to forecast future performance. It moves beyond simple observation to provide actionable business insights through time series forecasting. The project focuses on transforming raw temporal data into a stationary format to predict future trends using automated ARIMA modeling.

## 🚀 Project Objective
The goal is to take historical sales data, perform a full exploratory analysis, and implement an automated **ARIMA** pipeline to predict future sales trends with high statistical accuracy.

### 🛠️ Tech Stack & Libraries
* **Data Processing**: `Pandas`, `NumPy`
* **Visualizations**: `Matplotlib`
* **Statistical Testing**: `Statsmodels` (ADF Test)
* **Automated Modeling**: `pmdarima` (Auto-ARIMA)

## 📊 Analytical Workflow

### 1. Data Cleaning & Preparation
* **Handling Missing Data**: Identified and resolved gaps in the sales records to ensure a continuous time sequence.
* **DateTime Indexing**: Converted data into a time-series format by indexing on date columns.
* **Descriptive Statistics**: Generated a statistical summary to understand sales distribution and variance.

### 2. Exploratory Data Analysis (EDA)
* **Trend Analysis**: Visualized raw sales data to identify growth or decline patterns.
* **Rolling Statistics**: Calculated rolling mean and standard deviation to inspect variance stability over time.
* **Correlation Matrix**: Analyzed relationships between lagged sales variables.

### 3. Stationarity & Transformation
* **ADF Testing**: Performed the **Augmented Dickey-Fuller Test** to determine if the sales series was stationary.
* **Differencing**: Applied mathematical transformations to remove non-stationary trends, preparing the data for the model.

### 4. Forecasting Model (Auto-ARIMA)
* **Model Implementation**: Utilized the `pmdarima` library to automatically discover the best-fit parameters ($p, d, q$) for the sales forecast.
* **Model Summary**: Reviewed the statistical health of the model to ensure reliable predictions.
* **Future Forecast**: Generated a projected trend line showing expected future sales.

## 🔍 Key Findings (Results)
* **Trend Identification**: Confirmed a clear trend in sales volume that required transformation before modeling.
* **Stationarity Success**: Through differencing, the dataset's $p$-value was reduced, confirming the data became stationary and predictable.
* **Predictive Accuracy**: The model successfully captured historical sales cycles, allowing for a realistic projection of future sales growth.
