# Equity Portfolio Management

## Project Overview

This project focuses on managing a simulated equity portfolio based on historical data of 10 major stocks for the year 2018. The project implements and compares different trading strategies based on rebalancing periods and price trends, aiming to optimize the mark to market (MTM) value of the portfolio by the end of the year.

## Dataset

The dataset comprises daily closing and adjusted closing prices for the following stocks: IBM, MSFT, GOOG, AAPL, AMZN, FB, NFLX, TSLA, ORCL, SAP, for the entire year of 2018.

### Data Preparation

- **Download Data**: Historical daily data for each stock was downloaded from Yahoo Finance.
- **Dataframe Construction:** A dataframe was created with 20 columns representing the 'Close' and 'Adj Close' prices for each of the 10 stocks.
- **Initial Portfolio Setup:** Started with a $5 million fund, distributed equally among IBM, MSFT, GOOG, AAPL, and AMZN.

## Trading Strategies

- **5-Day Rebalancing of Buying Low:** Every 5 business days, the portfolio was adjusted to sell all holdings and buy shares of the 5 stocks that experienced the largest drop in 'Adj Close' prices.
- **5-Day Rebalancing of Buying High:** Every 5 business days, the strategy was adjusted to sell all holdings and buy into the 5 stocks whose 'Adj Close' prices increased the most.
- **Dividend Handling:** Accounted for dividends by adding dividend payouts directly to the cash account based on holdings on the dividend issue date.

## Analysis

- **High Tech Index Comparison:** The daily MTM of the portfolio was compared against a "high tech index", which represents the average 'Close' price of the 10 stocks.
- **Currency Conversion Impact:** Converted the MTM from USD to JPY using daily USD/JPY rates to analyze the impact of currency fluctuations.
- **Optimization:** Explored different rebalancing intervals to find the optimal frequency that maximizes the MTM by December 31, 2018.

## Results

- Plot of MTM and high tech index percentage changes over the year.
- Comparison of the two trading strategies in terms of performance.
- Analysis of how different rebalancing intervals affect portfolio value.

## Instructions

1. **Data Download Links:**
   - [Stock Data](https://finance.yahoo.com/)
   - [USD/JPY Historical Data](https://www.myfxbook.com/forex-market/currencies/USDJPY-historical-data)
2. **Setup:**
   - Ensure Python and necessary libraries (pandas, matplotlib) are installed.
   - Clone this repository and run the Jupyter Notebooks provided.

## Future Work

- Further refine trading algorithms based on machine learning predictions.
- Incorporate additional financial metrics for more nuanced trading decisions.
