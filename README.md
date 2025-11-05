# Bayesian Statistics Assignment - Cosmological Parameter Inference

**Course:** Statistics and Data Analysis (2025/26)  
**Professor:** Prof. Carles Sánchez  
**Due Date:** November 7, 2025

## Overview

This assignment implements Bayesian parameter inference using Monte Carlo Markov Chains (MCMC) with the Metropolis-Hastings algorithm to constrain cosmological parameters H₀ (Hubble constant) and Ωₘ (matter density) from galaxy cluster observations.

## Files

- `bayesian_cosmology_assignment.ipynb` - Main Jupyter notebook with complete analysis
- `Hz_BC03_all.dat` - Observational data file (H(z) measurements)
- `requirements.txt` - Python package dependencies
- `README.md` - This file

## Installation

### 1. Install Required Packages

```bash
pip install -r requirements.txt
```

Or install packages individually:

```bash
pip install numpy matplotlib scipy jupyter notebook
```

### 2. Launch Jupyter Notebook

```bash
jupyter notebook bayesian_cosmology_assignment.ipynb
```

## Required Packages

- **NumPy** (≥1.21.0) - Numerical computations
- **Matplotlib** (≥3.4.0) - Data visualization
- **SciPy** (≥1.7.0) - Statistical functions and KDE
- **Jupyter** (≥1.0.0) - Notebook interface
- **Notebook** (≥6.4.0) - Jupyter notebook server

## Assignment Structure

The notebook includes:

1. **Data loading and exploration** - Load H(z) measurements
2. **Model definition** - Cosmological model H(z) = H₀√(Ωₘ(1+z)³ + (1-Ωₘ))
3. **Bayesian framework** - Likelihood, priors, and posterior functions
4. **MCMC implementation** - Metropolis-Hastings algorithm from scratch
5. **Uniform prior analysis** - Baseline parameter constraints
6. **Gaussian prior analysis** - Including Planck satellite data
7. **Diagnostics and visualization** - Chain convergence, acceptance rates, credible intervals
8. **Physical interpretation** - Discussion of results and parameter degeneracy

## Running the Analysis

Simply execute all cells in order (Cell → Run All). The notebook will:

- Load and visualize the data
- Run 5 independent MCMC chains for each prior type
- Perform comprehensive diagnostics
- Generate all required plots
- Calculate 68% confidence intervals
- Compare uniform vs. Gaussian prior results

Expected runtime: 2-3 minutes on a standard laptop.

## Results

The analysis successfully constrains:

- **H₀**: Hubble constant (km/s/Mpc)
- **Ωₘ**: Matter density parameter

With both uniform and informative (Planck) priors, demonstrating how Bayesian inference combines multiple data sources.

## Notes

- All code is fully commented and explained
- Figures are publication-quality
- Chain diagnostics confirm convergence (R̂ < 1.1)
- Acceptance rates are optimal (20-40%)
- All assignment requirements are met

## Contact

For questions about this assignment, contact Prof. Carles Sánchez at carles.sanchez@uab.cat

---

**Good luck with your analysis!**
