# Sales Forecast Project

This project focuses on forecasting sales using the **perrin-freres-monthly-champagne-.csv** dataset. The primary aim is to analyze sales data and predict future trends using time series analysis techniques.

## Dataset
The dataset used is the **perrin-freres-monthly-champagne-.csv**, which contains monthly sales data for a champagne brand.

## Methods
To forecast sales, we have used the following models:

1. **ARIMA (AutoRegressive Integrated Moving Average)**: 
   - A time series forecasting method that combines three components:
     - **AutoRegressive (AR)**: Captures the relationship between a value and its lagged values.
     - **Integrated (I)**: Makes the time series stationary by differencing.
     - **Moving Average (MA)**: Models the relationship between the forecast and residual errors from previous time steps.

2. **SARIMA (Seasonal AutoRegressive Integrated Moving Average)**:
   - An extension of ARIMA that accounts for seasonality in the data.
   - It incorporates seasonal differencing and seasonal components to handle periodic patterns in the time series.

## Steps Performed
1. **Data Preprocessing**:
   - Handled missing values.
   - Visualized the data to understand trends and seasonality.

2. **Stationarity Check**:
   - Used techniques like the Augmented Dickey-Fuller (ADF) test to verify stationarity.

3. **Model Fitting**:
   - Fit ARIMA and SARIMA models to the dataset.
   - Tuned hyperparameters using techniques like Grid Search.

4. **Evaluation**:
   - Used metrics like Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) to evaluate model performance.
   - Compared ARIMA and SARIMA results to assess accuracy.

5. **Forecasting**:
   - Generated sales forecasts for future periods and visualized the results.

## Results
- The SARIMA model provided better predictions due to the presence of seasonal patterns in the data.
- Visualizations showed strong alignment between forecasted and actual values.

## Technologies Used
- Python
- Libraries: pandas, numpy, matplotlib, statsmodels, and scikit-learn

## How to Run the Project
1. Clone the repository.
2. Install the required libraries using:
   ```bash
   pip install -r requirements.txt
