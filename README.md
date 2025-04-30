# Crypto Options Pricing with Black-Scholes and Monte Carlo Simulation

This project explores the application of two foundational financial models — the Black-Scholes (B-S) model and Monte Carlo simulations — to price European-style call options for Bitcoin (BTC). Data was sourced directly from Deribit, one of the largest cryptocurrency options trading platforms.

The goal is to understand the performance and behavior of classical options pricing methods in the volatile, speculative landscape of crypto markets, and to evaluate how these models adapt under real-time market dynamics.

## Objectives

- Implement the Black-Scholes model (PDE-based) for European call options on BTC
- Simulate Geometric Brownian Motion and apply Monte Carlo (SDE-based) methods
- Compare both models to real market data from Deribit.com
- Assess how implied volatility and underlying asset shifts impact option pricing
- Visualize and interpret convergence of Monte Carlo pricing to B-S under increasing trial size

## Highlights

- Adapted classic models to BTC's unique market profile (zero risk-free rate, 24/7 trading, high volatility)
- Integrated Deribit's public API to retrieve real-time pricing and volatility data
- Developed scenarios to forecast price shifts and observe expected changes in option premiums
- Demonstrated model convergence and explained discrepancies through statistical reasoning

## Technologies Used

- Python
- NumPy
- Matplotlib
- pandas
- Deribit API
- SciPy

## Files

- `dataclass.py` — Handles API integration with Deribit
- `main_notebook.ipynb` — Implements both pricing models, analysis, and visualizations
- `utils/` — Includes any helper methods or formulas used during implementation

## Key Insights

- The Black-Scholes model, despite its limitations (e.g. constant volatility assumption), performed surprisingly well when compared with real option prices from Deribit.
- Monte Carlo simulations provided more flexibility in modeling stochastic behavior and demonstrated strong convergence to B-S prices with increased sample sizes.
- The project suggests strong potential for adapting traditional finance models to decentralized assets, and also opens the door to further exploration with stochastic volatility models like Heston.

## Next Steps

- Backtest trading strategies using historical data
- Integrate Heston model for better volatility handling
- Extend the model to support puts and alternative cryptocurrencies
- Compare outcomes across different option maturities and market regimes

---

This project was completed as part of an academic exploration into the intersection of financial mathematics, cryptocurrencies, and computational modeling.
