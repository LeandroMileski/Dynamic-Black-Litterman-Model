# Black-Litterman Portfolio Optimization
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Overview

This repository contains the implementation of my undergraduate thesis (*Trabalho de Conclusão de Curso*) titled **"Portfolio Optimization with the Black-Litterman Model: A Sectoral Portfolio Analysis in the United States"**, submitted to the Federal University of Santa Catarina (UFSC), Joinville Campus. The project explores the application of the Black-Litterman (BL) model to optimize sectoral investment portfolios based on the S&P 500, comparing two configurations—Restricted (MaxSharpe) and Unrestricted (LongShort)—against the S&P 500 benchmark.

The BL model combines market equilibrium returns (derived from CAPM) with investor views using a Bayesian approach, aiming to achieve superior returns while managing risk. This study uses historical data from 2005 to 2022, focusing on 10 U.S. economic sectors represented by ETFs, and includes backtesting to evaluate performance over a 10-year period (2014–2023).

### Key Results
- **MaxSharpe Portfolio**: Achieved a cumulative return of 245% over 10 years, with a Sharpe Ratio of 0.7818 and a Maximum Drawdown of -19.00%.
- **LongShort Portfolio**: Recorded a 174% cumulative return, with higher volatility (Sharpe Ratio: 0.6347, Maximum Drawdown: -29.00%).
- **S&P 500 Benchmark**: Returned 173%, with a Sharpe Ratio of 0.7395 and a Maximum Drawdown of -18.00%.

## Features

- **Data Collection**: Historical ETF data fetched via Yahoo Finance API (2005–2022).
- **Portfolio Optimization**: Implementation of the Black-Litterman model using PyPortfolioOpt, including the Exponential Weighted Covariance (EWC) method.
- **Backtesting**: Dynamic rebalancing over 10 years, with risk metrics (VaR, Sharpe Ratio, Maximum Drawdown, Standard Deviation).
- **Visualization**: Cumulative return plots and portfolio weight charts generated with Matplotlib and Plotly.

## Prerequisites

- **Python**: Version 3.7.13 (or compatible later versions).
- **Dependencies**:
  - `numpy` - Numerical computations.
  - `pandas` - Data manipulation.
  - `yfinance` - Financial data retrieval.
  - `PyPortfolioOpt` - Portfolio optimization.
  - `matplotlib` - Static visualizations.
  - `plotly` - Interactive visualizations.
  - `datetime` - Date handling.

Install dependencies using:
```bash
pip install -r requirements.txt

