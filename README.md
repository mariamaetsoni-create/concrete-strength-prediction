# Concrete Compressive Strength Prediction

## Problem
The compressive strength of concrete depends on its mix composition and age. Testing it in the lab takes days or weeks. This project builds a machine learning model that predicts the strength (in MPa) directly from the mix design.

## Data
Concrete Compressive Strength dataset (UCI / Kaggle): 1030 samples, 8 input variables (cement, blast furnace slag, fly ash, water, superplasticizer, coarse aggregate, fine aggregate, age) and 1 target (compressive strength in MPa). No missing values.

## Method
- Exploratory analysis with a correlation heatmap
- 80/20 train-test split
- Random Forest Regressor (300 trees)

## Results
- **R2 = 0.881**
- **Mean absolute error = 3.79 MPa**

Example: a mix with 350 kg/m3 cement, 175 kg/m3 water and age 28 days is predicted at **49.3 MPa**.

## Notebook
See `concrete_strength_prediction.ipynb`.

## Future improvements
- Compare with XGBoost and other models
- Hyperparameter tuning
- Build a small web app where users enter a mix and get the prediction
