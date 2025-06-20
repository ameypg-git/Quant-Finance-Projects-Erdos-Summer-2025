# Hypothesis Testing of Standard Assumptions in Theoretical Financial Mathematics

## Project Overview

In mathematical finance, it is commonly assumed that the log returns of financial assets are normally distributed. This project critically evaluates that assumption using historical market data for individual stocks, ETFs, and constructed portfolios.

Through a combination of visual diagnostics and formal statistical tests, we explore whether this assumption holds under various conditions, time periods, and asset combinations.

## Objectives

This project investigates the following key questions:

1. Do log returns of an index (e.g., S&P 500) exhibit normality in specific time windows?
2. Does removing periods of volatility improve the fit to a normal distribution?
3. Can we construct a portfolio of assets whose log returns are approximately normal?
4. Do previously constructed portfolios exhibit normality over different time frames?
5. Among a large set of stocks (S&P 500), which ones show evidence of normally distributed log returns?

## Methodology

- **Data Source:** Yahoo Finance (via `yfinance` library)
- **Period Analyzed:** Primarily 2023–2024 and 2020–2025 depending on section
- **Instruments:** S&P 500 ETF (VOO), major ETFs and stocks, low risk and high risk portfolios
- **Statistical Test Used:** D’Agostino–Pearson normality test (`scipy.stats.normaltest`)
- **Visualization:** Probability plots (QQ plots) to assess deviation from normality

## Key Findings

- **Time Sensitivity:** Log returns may appear normally distributed during calm market periods but fail normality tests during volatile periods.
- **Diversification Matters:** Broad based ETFs and well balanced portfolios tend to exhibit more normal like return distributions.
- **Portfolio Effects:** Both low risk and high risk portfolios may pass normality tests in the short term, but diverge over longer horizons.
- **Stock Universe Screening:** A small fraction of S&P 500 constituents exhibit return distributions that do not reject normality, offering candidates for Gaussian-based modeling.



