# 🧪 Perovskite Band Gap Prediction (EXCAVATE 2025)

This project was developed as part of the **EXCAVATE 2025** competition, where the objective was to classify and predict the **band gap** of **perovskite materials** using advanced machine learning techniques. The goal was to identify whether a material is an insulator and accurately estimate its band gap.

## Problem Statement

Given a dataset of perovskite materials with various atomic, orbital, and structural properties, the task is to:
- **Classify** materials as *insulators* or *non-insulators*.
- **Predict** the numeric value of their **band gap**.

## Methodology

### Feature Engineering
- `orbital_gap_A`, `orbital_gap_B`: Capture HOMO-LUMO gaps
- `charge_stability`: Charge neutrality for structural stability
- `adjusted_tolerance`: Geometric stability based on octahedral factors
- `EA_diff`: Electronegativity differences

### Models Used
- **XGBoost** for classification (Insulator vs Non-insulator)
- **CatBoost** for regression (Band gap value)

### Model Explainability
- **SHAP analysis**
- **Gain-based importance**
- **Permutation importance**

## Results

| Task         | Model     | Metric        | Value       |
|--------------|-----------|---------------|-------------|
| Classification | XGBoost   | Accuracy      | 94.47%      |
| Regression     | CatBoost  | R² Score      | 0.9017      |
|                |           | RMSE          | 0.2585      |

## Visualizations

- SHAP Summary Plots for both models
- Gain-based Feature Importance (XGBoost, CatBoost)
- Permutation Importance Charts
