#  Barrier Option Pricing with Gaussian Process Regression (GPR)

This project implements various methods to price a **down-and-out call barrier option**, combining **Monte Carlo simulation**, **Brownian Bridge correction**, and **Gaussian Process Regression (GPR)** for function approximation.

## 📄 Main File

| File            | Description |
|-----------------|-------------|
| `Barrier Option Pricing with GPR.ipynb` | Jupyter notebook containing the full implementation of pricing methods, GPR modeling, and sensitivity analysis (Delta, Gamma) |

## ⚙️ Methods Included

### 1. Standard Monte Carlo
Simulates the price paths of the underlying asset and evaluates the payoff if the barrier is not breached.

### 2. Brownian Bridge Correction
Improves accuracy by estimating the probability of barrier crossing between two monitoring dates.

### 3. Gaussian Process Regression (GPR)
Uses a non-parametric model (RBF kernel) to learn the pricing function  
\( f(S_0, K, B, \sigma, r) \) → *Option Price*

### 4. Sensitivity Analysis (Greeks)
- **Delta**: pathwise derivative with respect to \( S_0 \)
- **Gamma**: second-order pathwise derivative

## Required Libraries

- `numpy`
- `scipy`
- `matplotlib`
- `scikit-learn`

## Author

- **Aymane Mimoun**
- **Alexandre Combeau**
