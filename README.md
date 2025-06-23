# Quantitative Finance Projects : Erdős Institute Summer 2025

This repository contains a series of mini projects developed as part of the **Erdős Institute’s 2025 Introduction to Quantitative Methods in Finance**. Each project applies real world financial data, mathematical modeling, and programming techniques to explore practical questions in modern quantitative finance.

These projects demonstrate core competencies in financial data analysis, statistical testing, derivative pricing, and risk management under uncertainty : with a focus on rigorous quantitative methods , data analysis and  computational implementation.

---

## Projects Overview

### 1. Portfolio Optimization  
**Goal:** Construct and compare low risk and high risk portfolios using historical asset data.  
- Cleaned and analyzed 3 years of market data from Yahoo Finance.
- Computed returns, volatility, and correlations.
- Used `scipy.optimize.minimize` to generate optimized asset allocations under realistic constraints.
- Evaluated results using annualized volatility, expected return, and diversification metrics.

**Skills:** Portfolio theory, numerical optimization, data cleaning, visualization, real-market asset selection.

---

### 2. Hypothesis Testing of Return Normality  
**Goal:** Assess the assumption that asset log returns are normally distributed : a foundational concept in financial mathematics.  
- Tested normality of log returns for ETFs, stocks, and constructed portfolios.
- Applied statistical tests (D’Agostino–Pearson) and QQ plots across different time windows.
- Explored effects of volatility filtering, portfolio diversification, and asset selection.

**Skills:** Hypothesis testing, time-series diagnostics, statistical modeling, Python data science stack.

---

### 3. Black Scholes Option Pricing Analysis  
**Goal:** Examine how European option prices respond to changes in time to expiration and spot price.  
- Implemented the Black Scholes model for calls and puts.
- Visualized sensitivity to key parameters (Theta and Delta).
- Compared theoretical behavior between calls and puts using numerical derivatives.

**Skills:** Options pricing, derivatives theory, numerical analysis, financial visualization, modeling sensitivities.

---

### 4. Delta and Sigma Hedging under Stochastic Volatility  
**Goal:** Investigate the effectiveness of delta vs. vega (sigma) hedging under changing volatility conditions.  
- Simulated asset paths under both a stepwise volatility model and the Heston stochastic volatility model.
- Built delta only and vega neutral hedging strategies using call spreads.
- Analyzed P&L distributions and hedge frequency effects across scenarios.
- Compared simulated and theoretical prices for validation.

**Skills:** Derivative hedging, stochastic modeling, Monte Carlo simulation, Heston process, performance evaluation.

---

## Tools & Technologies

- **Languages**: Python
- **Core Libraries**: NumPy, pandas, Matplotlib, seaborn, SciPy, yfinance
- **Techniques**: Optimization, Monte Carlo simulation, hypothesis testing, volatility modeling, statistical inference
- **Frameworks**: Jupyter notebooks, modular Python functions (`functions.py`), visual diagnostics

---


