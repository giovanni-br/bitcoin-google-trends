# Cryptocurrency Price Dynamics and Google Trends Analysis

This repository contains the draft for a research project proposed in 2021. The research explores the relationship between investor attention, as measured by Google Trends, and the price dynamics of cryptocurrencies, specifically Bitcoin, Ethereum, and Litecoin. The study aims to evaluate how internet search trends can act as predictors for cryptocurrency prices, using various econometric and statistical methods.

## Research Overview

Cryptocurrencies have grown into a widely discussed topic in national and international media, especially after the 2017 price surges of Bitcoin. This project investigates the relationship between internet search data and cryptocurrency price behavior to understand how investor attention influences market dynamics.

### Objective

To evaluate the econometric/statistical characteristics of three major cryptocurrencies' price behavior and their relationship with search trends on Google. Specifically, the following were analyzed:

- Correlation (Pearson and Spearman)
- Stationarity
- Cointegration
- Granger Causality
- ARIMA and GARCH models (with and without search trend data)

### Data Sources

- **Google Trends**: Weekly search trend data for the terms "Bitcoin", "Ethereum", and "Litecoin".
- **CoinBase Pro**: Cryptocurrency price data for the respective cryptocurrencies.

## Methodology

The analysis was conducted using Python with the `statsmodels` library. The following steps were applied:

1. **Correlation Analysis**: To estimate the correlation between cryptocurrency prices and Google search trends, both Pearson and Spearman correlation coefficients were used.
2. **Stationarity Tests**: The Augmented Dickey-Fuller (ADF) and KPSS tests were applied to determine whether the time series data were stationary.
3. **Cointegration Testing**: Engel-Granger cointegration tests were performed to evaluate long-term relationships between the time series.
4. **Granger Causality**: Testing was conducted to assess whether search trends Granger-cause cryptocurrency price changes.
5. **ARIMA and GARCH Models**: Predictive models (ARIMA and GARCH) were implemented with and without the use of Google Trends data to evaluate their predictive capabilities.

## Results

- The analysis demonstrated a stronger performance of Spearman correlations, suggesting the possibility of non-linear relationships between cryptocurrency prices and search trends.
- Stationarity tests showed that most price and search trend data were non-stationary, but logarithmic returns were found to be stationary.
- Cointegration tests indicated long-term relationships between search trends and cryptocurrency prices (except for Litecoin returns).
- Granger causality tests showed the potential of Google Trends to forecast cryptocurrency price movements.

