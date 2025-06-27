# Mini Project 4: Delta and Sigma Hedging under Stochastic Volatility

**2025 Introduction to Quantitative Methods in Finance**  
**Erdös Institute**

---

## Objective

To understand how **time varying volatility** impacts the effectiveness of different hedging strategies in option pricing and risk management. We implement and compare **delta only** and **sigma (vega) hedging** approaches under both a simple stochastic volatility setup and the more realistic **Heston model**.

---

## Task Breakdown

### 1. Simulate Stock Paths
- **Toy Model**: Geometric Brownian motion with stepwise random volatility (σ ∈ {0.2, 0.3, 0.45}).
- **Heston Model**: Stochastic volatility simulated with mean reversion, volatility of volatility, and correlation to asset returns.

### 2. Implement Hedging Strategies
- **Delta Hedging**: Adjusts portfolio delta at each time step using estimated sigma.
- **Sigma Hedging**: Adds vega neutrality by constructing call spreads (short and long options).

### 3. Evaluate Performance
- Simulate profit and loss (P&L) distributions under each strategy.
- Analyze sensitivity to hedge frequency (1 to 252 times/year).
- Compare simulated vs. theoretical option prices.

---

## Deliverables

- `MiniProject4.ipynb`: Fully annotated Jupyter Notebook with simulations, code, and analysis.
- `functions.py`: Supporting library for pricing, Greeks, and simulation tools.

---

## Key Takeaways

- **Delta Hedging Alone is Incomplete**  
  Under stochastic volatility, delta hedging misses risk from volatility shocks, leading to potential under or over hedging.

- **Sigma (Vega) Hedging Improves Outcomes**  
  Adding a call spread hedge significantly improves P&L distribution, especially when the sold option is overpriced (i.e., implied > realized vol).

- **Hedge Frequency Matters**  
  More frequent hedging reduces variance and left tail risk. However, benefits diminish beyond ~50 hedges/year.

- **Heston Model Validates the Approach**  
  Both hedging methods approximate Heston model pricing well, but sigma hedging provides slightly tighter convergence to the theoretical value.
