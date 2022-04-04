# SBPproperties

© Copyright 2022 Tiago Morais

This repository includes the algorithm (Random Forest) that was developed to estimate pasture properties of Portuguese Sown biodiverse pastures rich in legumes (SBP) derived from Sentinel-2 data. The considered properties are:
- Standing biomass (kg/ha)
- Legumes fraction (-)
- Nitrogen content (g/kg)
- Phosphorus content (g/kg)

Used scripts are in folder "models" and the best trained models are in folder "trained_models"

Two cross-valiadtion approaches were used, whcih lead to set of models:
- Random cross-validation (RN-CV): random approach with random selection of the folds
- Leave-location-and-year-out cross-validation (LLYO-CV): each fold is the set of all observations from each farm and year

# Usage
- Requires scikit-learn library
- Requires joblib library
- Download folder "models" folder
- Prepare input data (see raw data file used in "Raw data folder"
- Use the individual models in the "models" folder using the input data file

# Reference
- Morais et al. (2022). **Characterization of Portuguese sown rainfed grasslands using remote sensing and machine learning.** *Precision Agriculture X(XX)*, XXX-XXX; (https://doi.org/10.1007/XX)
