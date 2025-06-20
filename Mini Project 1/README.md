
# Portfolio Optimization Project

A comparative analysis of low-risk and high-risk investment strategies using historical market data and quantitative optimization techniques.

---

## Objectives

- Construct two distinct portfolios: one low-risk and one high-risk.
- Use historical daily price data to compute returns, volatility, and asset correlations.
- Optimize portfolio allocations using realistic investment constraints.
- Evaluate portfolio performance using volatility, expected return, and diversification.

---

## Task Breakdown

1. **Data Collection**  
   - Download 3 years of daily price data using Yahoo Finance API.  
   - Assets chosen for each portfolio reflect their risk profiles (e.g., bonds for low-risk, tech stocks for high-risk).

2. **Data Processing**  
   - Calculate log returns, cumulative returns, and annualized volatility.  
   - Generate covariance and correlation matrices to assess asset relationships.

3. **Portfolio Optimization**  
   - Define constraints (e.g., 5%–40% or 10%–60% per asset).  
   - Use `scipy.optimize.minimize` to:
     - Minimize portfolio volatility (for low-risk portfolio).
     - Maximize expected return (for high-risk portfolio).

4. **Interpretation and Analysis**  
   - Justify asset selection and allocation strategy.  
   - Compare portfolios based on risk (volatility), return, and diversification.

---

## Deliverables

- **Jupyter Notebook (`MiniProject1 .ipynb`)**  
  Contains all code, commentary, visualizations, optimization routines, and results.

- **README.md**  
  This file, summarizing the project's goals, methodology, and outputs.

- **Portfolio Summary Tables**  
  Final asset weights, annualized volatility, and expected returns for both portfolios.

---

## Visualizations and Plots

- **Price Charts**: Raw asset prices and cumulative performance.
- **Heatmaps**: Covariance and correlation matrices for both portfolios.
- **Optimization Outputs**: Final weight allocations, volatility, and return metrics.
- **Integrated Markdown**: Clear explanations accompany each computational step.

---

This project demonstrates the application of financial theory, quantitative analysis, and real-world constraints in building and evaluating investment portfolios.
