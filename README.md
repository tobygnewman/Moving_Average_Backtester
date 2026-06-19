# Moving Average Crossover Strategy
## Overview

This project investigates whether a moving average crossover strategy can outperform a buy-and-hold approach after transaction costs.

The strategy was tested across multiple equities using historical daily price data from Yahoo Finance.

## Features
- Moving average crossover signals
- Transaction cost modelling
- Sharpe ratio analysis
- Maximum drawdown analysis
- Parameter optimisation
- Train-test validation
- Custom robustness scoring
- Strategy visualisation

## Methodology

The strategy enters a long position when the short moving average rises above the long moving average and exits when the opposite occurs.

Multiple parameter combinations were tested on training data (2015-2022).

The best-performing parameters were then evaluated on unseen test data (2022-2025).

A custom robustness score was also introduced to reward strong out-of-sample 
performance while penalising large deviations from training performance.

## Project Structure

- Data collection using Yahoo Finance
- Signal generation using moving average crossovers
- Backtesting framework with transaction costs
- Parameter optimisation
- Train-test validation
- Performance evaluation and visualisation

## Key Findings
- Results varied significantly across assets.
- Several securities underperformed buy-and-hold.
- Some assets demonstrated strong out-of-sample performance.
- Train-test validation helped reduce overfitting risk.

## Future Improvements
- Walk-forward optimisation
- Volatility targeting
- Portfolio-level testing
- Alternative technical indicators
