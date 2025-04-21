# Interpretable AI Model with LIME, SHAP, and NAM

This repository contains a project focused on building and interpreting an artificial neural network using various explainability techniques. The goal is to understand model behavior and feature influence using popular tools such as **LIME**, **SHAP**, and **NAM (Neural Additive Models)**.

## Model Architecture

The model is a feedforward neural network with the following configuration:

| Layer       | Config                                             |
|-------------|----------------------------------------------------|
| Linear      | input_dim=8, output_dim=100, activation=ReLU       |
| Batch Norm  | size=100                                           |
| Linear      | input_dim=50, output_dim=50, activation=ReLU       |
| Dropout     | p=0.2                                              |
| Linear      | input_dim=50, output_dim=50, activation=ReLU       |
| Linear      | input_dim=50, output_dim=20, activation=ReLU       |
| Linear      | input_dim=10, output_dim=1                         |

## Interpretability Techniques

Three different explainability methods were used to analyze the model:

- **LIME** (Local Interpretable Model-agnostic Explanations): Provides local explanations for individual predictions.
- **SHAP** (SHapley Additive exPlanations): Estimates feature contributions using game theory.
- **NAM** (Neural Additive Models): Enhances interpretability by modeling each feature with its own neural subnetwork.


