# Mini Project 4: Delta and Sigma Hedging under Stochastic Volatility

**Course**: Introduction to Quantitative Methods in Finance (2025)  
**Institution**: The Erdös Institute

## Overview

This project explores how non-constant volatility affects the performance of hedging strategies in options trading. Specifically, we simulate and evaluate:

- **Delta Hedging**: Hedging price risk by dynamically adjusting exposure to the underlying asset.
- **Sigma (Vega) Hedging**: Reducing volatility exposure using a call spread (selling one call, buying another).
  
We compare these strategies under two volatility models:

1. **Toy Model**: Geometric Brownian motion with discrete, randomly varying volatility.
2. **Heston Model**: A realistic stochastic volatility framework where volatility evolves continuously.

---

## Contents

- `functions.py`: Contains utility functions for Black-Scholes greeks, simulation, and hedging logic.
- `MiniProject4.ipynb`: Main notebook demonstrating simulations, visualizations, and analysis.
- `/images`: Histogram plots and comparison visuals for both models.

---

## Key Findings

- In the **toy model**, sigma hedging significantly reduces both risk and hedging error, outperforming delta-only hedging.
- Under the **Heston model**, both strategies perform well, but sigma hedging marginally improves pricing accuracy.
- Volatility risk is meaningful — incorporating vega hedging improves replication even in simplified markets.

---

## How to Run

1. Ensure Python 3.x environment with the following libraries:
   - `numpy`
   - `matplotlib`
   - `pandas`
   - `seaborn`
2. Run `MiniProject4.ipynb` in Jupyter Lab or Notebook.
3. Output plots and hedging performance will be shown for both models.

---

## Notes

- All simulations are Monte Carlo-based with configurable hedge frequency and volatility assumptions.
- The Heston model is implemented using Euler discretization and closed-form pricing for comparison.

---

## Author

*Submitted as part of the Erdös Institute Quantitative Finance Program.*

