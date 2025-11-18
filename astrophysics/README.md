# Galaxy Cluster Dark Matter Analysis: ACO 2670
## Estimating Virial Mass and Mass-to-Light Ratios with SDSS Data

This project analyzes the galaxy cluster ACO 2670 using photometric and spectroscopic data from the Sloan Digital Sky Survey (SDSS) Data Release 18 to estimate its virial mass and mass-to-light ratio. The analysis provides compelling evidence for the presence of dark matter and demonstrates computational techniques for studying large-scale cosmic structures.

### Background: Dark Matter and Galaxy Clusters

Dark matter represents approximately 27% of the universe's total mass-energy content, yet it doesn't interact electromagnetically and remains invisible to direct observation. Galaxy clusters, the largest gravitationally bound structures in the universe, serve as natural laboratories for studying dark matter because they contain vast amounts of it.

In 1933, Fritz Zwicky first discovered evidence for dark matter by observing that galaxies in the Coma Cluster were moving too fast to be held together by the visible matter alone. This "missing mass problem" suggested the presence of non-luminous matter. Today, we use similar techniques to study dark matter by comparing the total mass of clusters (inferred from galaxy motions) to their luminous mass (from starlight).

The mass-to-light (M/L) ratio serves as a key diagnostic: typical stellar populations have M/L ratios of 1-10 solar units, while dark matter-dominated clusters show ratios of 200-500 or higher. This dramatic difference reveals the invisible dark matter halo that dominates cluster mass.

### Key Features:

- **Multi-step iterative analysis**: Refines cluster membership through spatial and velocity constraints
- **Robust statistical methods**: Implements Bayesian Information Criterion for model selection and various binning algorithms
- **Relativistic corrections**: Uses proper cosmological distances rather than simple Hubble's Law approximations  
- **Comprehensive uncertainty analysis**: Propagates errors through all calculations using standard techniques
- **Advanced visualization**: Creates publication-quality plots showing spatial distributions, velocity dispersions, and luminosity profiles

### Technical Implementation:

#### Data Processing Pipeline:
1. **Cluster Member Selection**: Iterative refinement using 1.5 Mpc radial cutoff and ±3σ redshift clipping
2. **Weighted Center Calculation**: Uses inverse-variance weighting based on photometric uncertainties
3. **Redshift Analysis**: Compares single Gaussian vs. Gaussian Mixture Models using BIC
4. **Distance Calculations**: Implements relativistic Doppler corrections and ΛCDM cosmology
5. **Spatial Analysis**: Computes projected distances with proper coordinate system corrections

#### Physical Measurements:
- **Velocity Dispersion**: Fits Gaussian distributions to peculiar velocities with outlier detection
- **Luminosity Analysis**: Calculates absolute magnitudes and converts to solar luminosity units  
- **Effective Radius**: Determines half-light radius accounting for projection effects
- **Virial Mass**: Applies virial theorem using velocity dispersion and spatial scale
- **Mass-to-Light Ratio**: Combines dynamical mass with photometric luminosity

### Results and Significance:

The analysis yields a virial mass of (8.03 ± 2.49) × 10¹⁴ M☉ and an extremely high mass-to-light ratio of 441 ± 137 M☉/L☉. This ratio is nearly two orders of magnitude higher than typical stellar populations, providing strong evidence that ACO 2670 is dominated by dark matter.

The cluster shows signs of dynamical activity with mild kinematic asymmetries, suggesting recent merger activity or ongoing accretion. Despite this complexity, the redshift distribution remains well-described by a single Gaussian, indicating the system is largely virialized.

### Applications and Broader Impact:

This type of analysis serves multiple purposes in modern astrophysics:

- **Cosmological Parameter Estimation**: Cluster masses help constrain dark matter density and structure formation models
- **Galaxy Evolution Studies**: Understanding how galaxies behave in dark matter-dominated environments  
- **Dark Matter Physics**: Testing alternative theories of gravity and dark matter interactions
- **Large-Scale Structure**: Mapping the cosmic web through cluster mass measurements

The computational techniques demonstrated here are widely applicable to analyzing massive datasets from current and future astronomical surveys, making this both a scientific investigation and a practical demonstration of astronomical data analysis methods.

### Prerequisites:

- Python proficiency with NumPy, SciPy, Matplotlib, and Astropy
- Basic understanding of statistics (error propagation, fitting, hypothesis testing)
- Familiarity with astronomical concepts (redshift, magnitudes, coordinate systems)
- Knowledge of SQL for database queries (SDSS data access)

This project serves as both a complete scientific analysis and an educational example of how computational methods reveal fundamental properties of the universe's dark components.
