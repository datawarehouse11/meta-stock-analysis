# Meta Inc. (META) Stock Price Analysis and Forecasting

[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.x](https://img.shields.io/badge/python-3.x-blue.svg)](https://www.python.org/downloads/)
[![Libraries](https://img.shields.io/badge/Libraries-Pandas%20%7C%20YFinance%20%7C%20Matplotlib%20%7C%20Statsmodels%20%7C%20Scikit--learn-brightgreen)](https://pypi.org/)

## Overview

This repository contains a Python-based project focused on analyzing and forecasting the stock price of Meta Platforms, Inc. (ticker symbol: META). The current analysis provides a foundational understanding of the stock's historical performance and utilizes an Autoregressive Integrated Moving Average (ARIMA) model for short-term price prediction.

This project serves as a starting point, with plans for future expansion to include more advanced analytical techniques and a deeper exploration of factors influencing Meta's stock price in a separate, more in-depth notebook.

## Current Analysis (Notebook: `financial performance analysis of Meta Inc.ipynb`)

The initial analysis notebook (`financial performance analysis of Meta Inc.ipynb`) covers the following key steps:

* **Data Acquisition:** Downloading historical stock price data for Meta Inc. from Yahoo Finance, spanning from January 2021 to December 2024.
* **Data Preprocessing:** Handling missing daily stock data using linear interpolation to create a continuous time series suitable for analysis.
* **Exploratory Data Analysis (Initial):**
    * Visualizing the historical trend of Meta's stock price over the downloaded period.
    * Calculating and presenting key financial ratios (Profit Margin, Debt-to-Equity Ratio, Return on Equity) based on available financial statements to provide a broader financial context.
    * Examining year-over-year revenue growth.
* **Time Series Forecasting (ARIMA Model):**
    * Implementing an ARIMA(5,1,0) model to forecast the stock price for a 30-day horizon.
    * Visualizing the forecasted price against the recent historical data.
* **Model Evaluation:**
    * Evaluating the performance of the fitted ARIMA model by predicting the stock price for the last 30 days of the dataset.
    * Quantifying the model's accuracy using the Root Mean Squared Error (RMSE).
    * Providing a visual comparison of the actual versus predicted stock prices for the evaluation period.

## Planned Future Work (In-depth Analysis - Separate Notebook)

A subsequent, more in-depth analysis will be conducted in a separate notebook and will aim to provide a more comprehensive understanding through:

* **Advanced Exploratory Data Analysis:**
    * Detailed trend analysis of key financial ratios over time.
    * Correlation analysis between different financial metrics and the stock price.
    * Stock price decomposition into trend, seasonality (if applicable), and residual components.
    * Volatility analysis.
* **Robust Model Selection and Comparison:**
    * Formal stationarity testing of the time series data.
    * Utilizing Autocorrelation Function (ACF) and Partial Autocorrelation Function (PACF) plots to inform ARIMA order selection.
    * Model diagnostics and residual analysis.
    * Potential comparison with other time series forecasting models (e.g., SARIMA for seasonality, Exponential Smoothing).
* **Incorporating External Factors:**
    * Exploration of potential external variables that may influence Meta's stock price (e.g., market indices, competitor performance, news sentiment).
    * Consideration of multivariate time series models or machine learning approaches to incorporate these factors.
* **Enhanced Evaluation and Validation:**
    * Implementing train-validation-test splits for more rigorous model evaluation.
    * Employing backtesting techniques (e.g., rolling forecasts) to assess out-of-sample performance.
    * Potentially providing confidence intervals for forecasts.

## Getting Started

1.  **Prerequisites:** Ensure you have Python 3.x installed on your system. You can download it from [https://www.python.org/downloads/](https://www.python.org/downloads/).
2.  **Installation:** Install the necessary Python libraries using pip:
    ```bash
    pip install pandas yfinance matplotlib statsmodels scikit-learn
    ```
3.  **Running the Code:**
    * Clone this repository to your local machine:
        ```bash
        git clone [https://github.com/datawarehouse11/your-repo-name.git](https://github.com/datawarehouse11/your-repo-name.git)
        cd your-repo-name
        ```
        (Replace `your-repo-name` with the actual name of your repository).
    * Open the `financial performance analysis of Meta Inc.ipynb` file using Jupyter Notebook or JupyterLab.
    * Run the cells sequentially to execute the analysis and generate the forecast.

## Contributing

While this is primarily a personal project, any suggestions or feedback on the analysis or potential improvements are welcome.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

Waydin Josephs (datawarehouse11)

---
