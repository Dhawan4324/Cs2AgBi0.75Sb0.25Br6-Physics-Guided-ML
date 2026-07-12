# High-Dimensional Physics-Guided Machine Learning for Interpretable Optimization of Lead-Free Cs₂AgBi₀.₇₅Sb₀.₂₅Br₆ Double-Perovskite Solar Cells

This repository contains the machine-learning workflow, simulation dataset, model-evaluation results, interpretability analysis, and optimized device conditions associated with the study:

**“High-Dimensional Physics-Guided Machine Learning for Interpretable Optimization of Lead-Free Cs₂AgBi₀.₇₅Sb₀.₂₅Br₆ Double-Perovskite Solar Cells.”**

## Repository File

### `Cs₂AgBi₀_₇₅Sb₀_₂₅Br₆_Model.ipynb`

This Jupyter Notebook contains the complete machine-learning workflow developed for the high-dimensional analysis and optimization of the proposed double-perovskite solar cell.

The notebook includes:

- Dataset import and inspection
- Data cleaning and preprocessing
- Feature and target-variable selection
- Training and testing data separation
- Machine-learning model development
- Cross-validation and performance evaluation
- Predicted-versus-simulated analysis
- Feature-importance and interpretability analysis
- Prediction of optimized device conditions
- Validation of the machine-learning-predicted conditions using SCAPS-1D

## Input Parameters

The machine-learning dataset includes the following device parameters:

- Absorber bulk defect density, \(N_t\)
- Absorber electron affinity, \(\chi\)
- Absorber acceptor density, \(N_A\)
- Absorber thickness
- Electron transport layer/absorber interface defect density
- Hole transport layer/absorber interface defect density
- Operating temperature
- Series resistance, \(R_s\)
- Shunt resistance, \(R_{sh}\)

## Target Variables

The predicted photovoltaic parameters are:

- Open-circuit voltage, \(V_{OC}\)
- Short-circuit current density, \(J_{SC}\)
- Fill factor, FF
- Power conversion efficiency, PCE

## Machine-Learning Models

The notebook evaluates the following regression models:

- Linear Regression
- Random Forest Regression
- Extreme Gradient Boosting Regression
- Artificial Neural Network

## Performance Interpretation

The physically realistic SCAPS-1D-optimized device achieved a PCE of **24.07%**.

The machine-learning-predicted and SCAPS-validated best-case condition achieved a PCE of **27.23%**. This value represents an upper-performance-limit condition within the investigated high-dimensional simulation space.

## Requirements

The notebook requires Python 3 and the following main libraries:

```text
numpy
pandas
matplotlib
scikit-learn
xgboost
tensorflow
joblib
openpyxl
shap
