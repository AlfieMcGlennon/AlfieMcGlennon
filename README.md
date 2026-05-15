# Alfie McGlennon

MSc Climate Change & Artificial Intelligence at the University of Reading. Researching compound heat stress risk across Europe using copula-based statistical frameworks and machine learning.

My dissertation builds a multiplicative decomposition of compound hazard bias (M_total = M_marginal × M_dependence), then uses XGBoost to predict Kendall's τ dependence from large-scale atmospheric circulation patterns. The goal is to separate where climate model errors come from in multivariate extremes, and whether ML can correct the dependence structure directly. Working with ERA5 reanalysis, CMIP6 projections, and Destination Earth (DestinE) climate digital twin data.

Targeting roles in climate risk analytics, reinsurance (Swiss Re, Munich Re), and operational meteorology (ECMWF and adjacent).

## What I've been building

**Compound heat stress risk modelling** · Copula-based bivariate framework for temperature and humidity extremes across European regions. Marginal fitting, dependence estimation via Kendall's τ, and ML-driven bias decomposition. Python, xarray, scipy, scikit-learn, XGBoost.

**[GB Grid Scenario Tool](https://github.com/AlfieMcGlennon/gb-grid-tool)** · Interactive transmission grid model built from public NESO data. 27 TNUoS zones, 82 FLOP zones, 43 transmission links, 18 ETYS boundaries. DC power flow with real backbone reactances. Three dispatch modes including an LP solver compiled to WebAssembly. Weather driven by 34 years of ERA5 reanalysis. Validated against NESO published transfer capabilities (B6F within 2%) and cross-validated against PyPSA-GB. Runs entirely in the browser.

**RL grid dispatch agents** · Trained PPO agents (Stable Baselines3) on 9 years of real GB generation, wholesale price, and ERA5 weather data to learn dispatch strategies from scratch. Explored MLP, CNN, and 27-zone zonal architectures with DC power flow constraints. 10M+ timestep training runs on SLURM (University of Reading RACC HPC cluster). Agents went from spending £30B/year to within 6% of real grid operations through iterative reward design.

**Quantum ML for atmospheric regression** · Variational quantum circuits (PennyLane) applied to ERA5 temperature fields and the Lorenz '63 system. Central contribution: Fourier decomposition as an interpretability tool for per-qubit structured VQC regression, with trainable per-feature encoding. Depth sweeps, noise ablations, and cross-validation on chaotic dynamics.

**[Climate Data Quickstart](https://github.com/AlfieMcGlennon/climate-data-quickstart)** · Open-source toolkit covering 14 climate datasets including ERA5 variants, HadCET, CMIP6, UKCP18, GloFAS, and Earth Data Hub. Built using a three-stage agentic pipeline.

**[City Climate Stripes](https://github.com/AlfieMcGlennon/city-climate-stripes)** · Interactive temperature anomaly visualisation by season and year, inspired by Ed Hawkins' warming stripes.

**Electricity demand forecasting (India)** · ML models (linear regression, XGBoost, LSTM) for state-level demand prediction using weather variables. Temporal cross-validation methodology with per-state R² choropleth mapping.

## Technical stack

**Languages:** Python (primary), JavaScript/TypeScript, HTML/CSS, Bash

**ML & stats:** XGBoost, scikit-learn, Stable Baselines3 (PPO), LSTM/PyTorch, PennyLane (quantum ML), copula methods, scipy, statsmodels

**Climate & geo:** xarray, netCDF4, cdsapi, cfgrib, cartopy, ERA5, CMIP6, UKCP18, GloFAS, DestinE

**Infrastructure:** SLURM (HPC job scheduling), Linux, Git, Obsidian, LaTeX

**Web:** React, Leaflet, D3.js, WebAssembly, GitHub Pages

## Connect

- [LinkedIn](https://www.linkedin.com/in/alfred-mcglennon-927589253/)
- University of Reading, Department of Meteorology
