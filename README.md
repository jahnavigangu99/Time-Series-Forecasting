# Time-Series-Forecasting Projects

Welcome to the repository! This collection of time series forecasting and analysis projects focuses on real-world economic and financial data, with methods like ARIMA, Holt-Winters, and state-space models. These projects involve the imputation of missing values during the COVID-19 pandemic and analysis using exogenous variables such as unemployment rates.

### Projects Overview

1. **GDP Forecasting**  
   This project forecasts GDP using advanced time series modeling techniques, including AutoARIMA and ETS models. The dataset is retrieved from FRED (Federal Reserve Economic Data) and analyzed for missing data points, which are imputed using interpolation techniques. A K-fold cross-validation is used to assess the model performance.

   **Key Techniques**:
   - AutoARIMA model fitting
   - ETS model analysis
   - Model residual analysis (ACF/PACF)
   - K-fold cross-validation for forecast accuracy evaluation

   **Results**: Both AutoARIMA and ETS models were used to predict GDP with cross-validation for validation. The models' performance was evaluated based on RMSE, MAE, and MAPE.

2. **Time Series Analysis with Exogenous Variables: ICNSA and UNRATE**  
   This project analyzes and forecasts Initial Claims for Unemployment (ICNSA) using unemployment rate (UNRATE) as an exogenous variable. ARIMA models are implemented with the integration of exogenous variables to capture the relationship between the two datasets.

   **Key Techniques**:
   - ARIMA modeling with exogenous variables (UNRATE)
   - Cross-correlation analysis
   - Stationarity testing using the Augmented Dickey-Fuller (ADF) test
   - Model diagnostics and residual checks

   **Results**: A regression with ARIMA errors was used to forecast ICNSA with UNRATE as a covariate. The final model provided insights into how unemployment rates influence initial claims for unemployment.

3. **COVID-19 Value Imputation in Time Series Data**  
   This project focuses on handling missing values during the COVID-19 pandemic in time series datasets. A state-space model was used to dynamically impute missing values during the pandemic, considering both seasonal and trend components.

   **Key Techniques**:
   - State-space modeling for imputation
   - Handling missing data during the COVID-19 period
   - Visual comparison of original and imputed data

   **Results**: The imputation was successfully applied to fill gaps caused by the COVID-19 pandemic. The state-space model helped maintain the continuity of the data, preserving trends and seasonality.

### Repository Structure

- **GDP_forecast.pdf**: This file contains the detailed analysis and forecasting of GDP using time series models.
- **TimeSeries_Analysis.pdf**: A comprehensive time series analysis involving ICNSA and unemployment rate (UNRATE) data, with ARIMA and cross-correlation analysis.
- **CovidValueImputation.pdf**: Documentation of value imputation techniques for time series data affected by the COVID-19 pandemic.

### How to Run

1. **Install the Required Libraries**:
   ```r
   install.packages(c("tidyverse", "fredr", "forecast", "imputeTS", "tseries", "bsts"))
   ```

2. **Run the Analysis**:  
   Clone the repository and execute the R scripts provided in each project folder. Follow the steps in the PDF reports for detailed insights.

### Contributions

Feel free to contribute to this repository by submitting pull requests, raising issues, or providing feedback.
