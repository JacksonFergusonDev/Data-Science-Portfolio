# Exoplanet Atmospheric Analysis: Characterizing Structure and Composition from Descent Probe Data

## Abstract
This project analyzes data from five atmospheric descent probes on a high-gravity exoplanet ($g = 20 \text{m/s}^2$) to reconstruct atmospheric properties, composition, and dynamics. The analysis reveals a nitrogen-dominated atmosphere with helium, argon, CO₂, and spatially variable water vapor content.

---

## Background
Atmospheric descent probes directly measure temperature, pressure, density, and composition throughout planetary atmospheres.  
This exoplanet's doubled surface gravity fundamentally alters atmospheric structure, compressing layers and affecting scale height, pressure gradients, and convection patterns.

---

## Key Features
- **Multi-probe validation**: Five independent probes ensure measurement consistency  
- **Temperature reconstruction**: Recovers damaged sensor data via hydrostatic equilibrium  
- **Composition analysis**: Calculates molecular abundances and thermodynamic properties  
- **Radiative transfer**: Determines optical depths for CO₂ and H₂O absorption  
- **Hydrological modeling**: Estimates precipitation rates and water residence times  

---

## Technical Implementation

### Data Processing
- Converts molecular number densities to mass fractions  
- Validates hydrostatic equilibrium using finite differences  
- Reconstructs missing temperature data  
- Calculates specific humidity, relative humidity, and vapor pressure profiles  

### Physical Measurements
Key results include:
- Precipitable water: **36–48 kg/m²**  
- Mixture heat capacity: **800–1300 J/kg/K**  
- Potential temperature profiles for stability analysis  
- Optical depth integration using Beer–Lambert law  

Surface optical depth reaches **τ ≈ 4.6–4.9**, dominated by CO₂ absorption.

---

## Results and Significance
- Excellent inter-probe agreement validates methodology:  
  - At **450 hPa**, temperatures vary only **0.57 K** (228.16–228.73 K)  
- Precipitable water shows **31% spatial variability** (36.2–47.5 kg/m²), indicating active circulation or regional moisture differences  
- Global precipitation rate: **0.096 ± 0.014 mm/hour**  
- Atmospheric water residence time: **32.6 ± 5.6 years**  
  - Much slower than Earth’s ~9-day cycle due to high gravity suppressing evaporation  

---

## Applications
- **Comparative planetology**: Understanding gravity’s effect on atmospheric structure  
- **Climate modeling**: Providing validation data for circulation models  
- **Habitability assessment**: Characterizing water availability and greenhouse warming  
- **Mission design**: Demonstrating value of multiple descent probes  

---

## Prerequisites
- Python with **NumPy, SciPy, Matplotlib**  
- Knowledge of atmospheric physics:  
  - Hydrostatic equation  
  - Thermodynamics  
  - Radiative transfer  
- Error propagation techniques  
- Basic fluid dynamics  

---

## Conclusion
This analysis demonstrates how fundamental physics combined with careful data processing reveals both familiar atmospheric processes and exotic differences driven by altered planetary conditions.
