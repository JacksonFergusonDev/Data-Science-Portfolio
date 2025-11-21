# Computational Statistics Portfolio

[![Return to Portfolio](https://img.shields.io/badge/⬅️_Back_to-Main_Portfolio-grey)](../README.md)
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![SciPy](https://img.shields.io/badge/SciPy-Statistics-orange)
![NumPy](https://img.shields.io/badge/NumPy-Computation-green)

**A collection of statistical analysis projects demonstrating hypothesis testing, parameter estimation, and Monte Carlo simulation techniques.**

> 🚧 **Currently Refactoring** - This section is being consolidated into a single, streamlined notebook (`computational_statistics_portfolio.ipynb`) with an improved data pipeline structure. Individual notebooks below will be replaced once refactoring is complete.

---

## 🎯 Project Overview
This collection demonstrates core statistical methods and computational techniques used in data science and scientific computing. Each project showcases a different aspect of statistical inference, from hypothesis testing and sampling methods to parameter estimation and uncertainty quantification.

**Scope:** The projects use synthetic datasets and simulated experiments to illustrate fundamental statistical concepts without the complexity of real-world data noise, making the underlying principles more transparent.

---

## 📊 Key Visualizations

### Statistical Inference & Validation
*Demonstrations of parameter estimation, uncertainty quantification, and theoretical validation through simulation.*

<p float="left">
  <img src="images/model_comparison.png" width="48%" />
  <img src="images/b_hat_distribution.png" width="48%" /> 
</p>

* **Left:** Model Fit Validation. Comparison of synthetic data (with error bars) against an optimized model fit using chi-square minimization. The residuals indicate the quality of the parameter estimation.
* **Right:** Monte Carlo Parameter Distribution. Distribution of the estimated parameter *b* across 1000 trials. The Gaussian shape confirms the validity of the error estimation methods and demonstrates the Central Limit Theorem in action.

### Probability & Convergence
*Exploration of the Central Limit Theorem and the behavior of sum-variables.*

<p float="left">
  <img src="images/z2_z3_z6_histograms.png" width="48%" />
</p>

* **Center:** Central Limit Theorem Demonstration. Histograms of sum-variables (Z₂, Z₃, Z₆) showing progressive convergence toward a Normal distribution as sample size increases, as predicted by theory.

---

## 🛠️ Technical Implementation

The analysis is built in **Python** using NumPy and SciPy, with emphasis on implementing statistical algorithms from first principles rather than relying on black-box libraries.

### Hypothesis Testing & Sampling
* **PDF Normalization:** Calculates normalization constants for arbitrary probability density functions using numerical integration.
* **Critical Value Determination:** Implements hypothesis testing framework with Type I error control at 95% confidence level.
* **Specialized Sampling Methods:** 
  - Inverse transform sampling for standard distributions
  - Accept-reject algorithm for complex PDFs
* **Error Rate Analysis:** Empirical measurement of Type I and Type II error rates through simulation.

### Parameter Estimation
* **Chi-Square Minimization:** Implements least-squares fitting for model parameter estimation with non-uniform error bars.
* **Uncertainty Quantification:** Calculates parameter uncertainties from the Hessian matrix at the minimum.
* **Monte Carlo Validation:** Validates uncertainty estimates through 1000 replicate experiments.
* **Pull Distribution Analysis:** Verifies that estimated uncertainties are correctly calibrated.

### Maximum Likelihood Estimation
* **Geometric Problem:** Analyzes distances between random points on parallel rods to estimate rod length.
* **Analytical Derivation:** Derives theoretical PDF from geometric constraints.
* **MLE Implementation:** Finds maximum likelihood estimator and quantifies uncertainty using Fisher information.
* **Bootstrap Validation:** Confirms estimator properties through 1000 bootstrap replications.

### Probability Theory
* **Distribution Simulation:** Generates samples from various probability distributions and compares to theoretical predictions.
* **Correlation Analysis:** Demonstrates generation of correlated random variables through common factors.
* **Empirical Validation:** Compares simulated covariance and correlation coefficients against theoretical values.

---

## 📂 Project Structure

### Consolidated Portfolio (In Progress)
**[computational_statistics_portfolio.ipynb](computational_statistics_portfolio.ipynb)** - Unified notebook with improved data pipeline combining all projects below.

### Individual Projects (Being Consolidated)

#### 1. Hypothesis Testing Simulation
**[hypothesis_testing_simulation.ipynb](hypothesis_testing_simulation.ipynb)**
- Implementation of competing probability distributions (H0 vs H1)
- Inverse transform and accept-reject sampling methods
- Empirical error rate analysis

#### 2. Statistical Distance Analysis
**[statistical_distance_analysis.ipynb](statistical_distance_analysis.ipynb)**
- Maximum likelihood estimation for geometric problem
- Uncertainty quantification via numerical and analytical methods
- Bootstrap validation of estimator properties

#### 3. Parameter Estimation & Validation
**[parameter_estimation.ipynb](parameter_estimation.ipynb)**
- Chi-square minimization for model fitting
- Hessian-based uncertainty calculation
- Monte Carlo validation and pull distribution analysis

#### 4. Random Variable Simulation
**[statistical_analysis_simulation.ipynb](statistical_analysis_simulation.ipynb)**
- Central Limit Theorem demonstration
- Correlated random variable generation
- Empirical validation of theoretical statistics

---

## 🚀 Quick Start

This project is part of my Data Science Portfolio. To reproduce the analysis:

1. **Clone the portfolio repository:**
```bash
   git clone https://github.com/JacksonFergusonDev/Data-Science-Portfolio.git
   cd Data-Science-Portfolio
```

2. **Install shared dependencies:**
```bash
   pip install -r requirements.txt
```

3. **Launch the Computational Modeling analysis:**
```bash
   cd computational_modeling
   jupyter notebook computational_statistics_portfolio.ipynb
```
   *(Or explore individual notebooks while refactoring is in progress)*

---

### Author
**Jackson Ferguson** | Astrophysics Undergraduate, University of Victoria  
[GitHub Profile](https://github.com/JacksonFergusonDev) | [LinkedIn](https://linkedin.com/in/jackson--ferguson/)