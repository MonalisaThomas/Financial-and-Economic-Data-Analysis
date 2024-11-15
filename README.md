# Portfolio Optimization with ETFs (SPY & TLT)

This project performs portfolio optimization on two popular ETFs: SPY (S&P 500 Index) and TLT (Long-Term Treasury Bonds). The objective is to find the optimal weights for a portfolio that maximizes the Sharpe ratio, which is a measure of risk-adjusted return.

## Project Overview

The script downloads daily price data for the ETFs from Yahoo Finance, normalizes the data, and visualizes price trends. It then calculates optimal weights for the portfolio based on historical returns and risks, aiming to achieve the highest Sharpe ratio.

### Key Features

- **Data Download and Preprocessing**: Fetches adjusted closing prices for SPY and TLT from Yahoo Finance, starting from January 1, 2010.
- **Normalization**: The price series for each ETF is normalized to a starting value of $100 to allow comparison.
- **Visualization**: Plots normalized prices, highlighting the maximum and minimum price points.
- **Portfolio Optimization**:
  - Uses `scipy.optimize.minimize` to maximize the Sharpe ratio.
  - Applies constraints (weights sum to 1) and bounds (0 ≤ weights ≤ 1).
- **Result Output**: Displays the optimal portfolio weights for SPY and TLT.

## Requirements

- Python 3.x

### Required Libraries
- `pandas`
- `numpy`
- `yfinance`
- `matplotlib`
- `scipy`

To install the necessary libraries, run:

```bash
pip install pandas numpy yfinance matplotlib scipy


