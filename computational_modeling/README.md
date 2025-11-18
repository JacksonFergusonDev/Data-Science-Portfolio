# Computational Modeling and Analysis
## Hypothesis Testing Simulation with Critical Value Analysis

This project demonstrates fundamental concepts of statistical hypothesis testing through simulation. The code implements and analyzes two competing probability distributions (H0 and H1) to explore statistical error rates and sampling methods.

### Key Features:
- Calculation of normalization constants for probability density functions
- Determination of critical value for a 95% confidence level hypothesis test
- Implementation of specialized sampling techniques:
  - Inverse transform sampling for H0
  - Accept-reject method for H1
- Empirical measurement of Type I and Type II error rates
- Visual comparison of theoretical PDFs against generated sample distributions

This project serves as a practical demonstration of hypothesis testing fundamentals, sampling methodologies, and error analysis in statistics. It's particularly useful for students learning statistical inference, researchers implementing custom statistical tests, or practitioners interested in the empirical performance of different sampling techniques.

## Statistical Distance Analysis Between Uniform Random Points

This project demonstrates statistical inference techniques by analyzing the distances between random points on two parallel rods. The implementation includes:

### Key Features:
- Simulation of random points on parallel rods with specified geometry
- Derivation and visualization of the theoretical probability density function
- Maximum likelihood estimation of rod length from distance measurements
- Uncertainty quantification using both numerical and analytical second derivatives
- Bootstrap validation through 1000 replicate experiments
- Analysis of estimator bias and variance

This code serves as an educational example for probability theory, statistical inference, and computational physics. It illustrates the practical application of maximum likelihood methods with complete uncertainty analysis, making it useful for students and researchers in statistics, physics, or quantitative fields dealing with geometric probability problems.

## Parameter Estimation and Statistical Validation

This project demonstrates a complete workflow for parameter estimation and statistical validation using synthetic data. The code simulates a physical system with the model function `a*t*cos(b*t)`, estimates parameters via chi-square minimization, and validates the statistical properties of the estimation process.

### Key Features:
- Generation of synthetic data with non-uniform error bars
- Parameter estimation using chi-square minimization
- Uncertainty calculation from the Hessian matrix
- Monte Carlo validation of parameter estimates (1000 replications)
- Pull distribution analysis to verify uncertainty estimates
- Chi-square distribution analysis to confirm proper fit statistics

This project serves as a template for rigorous parameter estimation in scientific data analysis, particularly useful for physics, astronomy, or any field requiring model fitting with proper uncertainty quantification and statistical validation.

## Statistical Analysis and Simulation of Random Variables

This project explores statistical concepts through simulation and visualization. It consists of two main parts: a match outcome simulator and an exploration of the Central Limit Theorem and correlated random variables.

### Key Features:
- Simulation of game outcomes (wins/losses/draws) with fixed probabilities
- Statistical comparison between theoretical and empirical distributions
- Visualization of bivariate relationships with and without added noise
- Demonstration of the Central Limit Theorem with different sample sizes
- Generation and analysis of correlated random variables through common factors
- Empirical validation of theoretical covariance and correlation coefficients

This project serves as a practical introduction to statistical simulation concepts. It demonstrates how to generate random outcomes according to specific distributions, analyze their statistical properties, and visualize relationships between variables. The code is particularly useful for students learning probability theory, researchers needing example implementations of random variable generation, or data scientists interested in understanding correlation structures through simulation.
