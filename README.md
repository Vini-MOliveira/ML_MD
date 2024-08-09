
# ML_MD: A Tool to Distinguish Conformational States Using Residue Pair Energies

## Overview
This repository contains a machine learning (ML) tool designed to analyze molecular dynamics (MD) trajectories to distinguish between different conformational states of proteins. The tool calculates residue pair interaction energies, including hydrogen bonds and π-π interactions, to identify and differentiate conformational states.

## Introduction
Understanding protein conformational states is critical for insights into their functional mechanisms. This tool leverages MD trajectories and applies ML techniques to calculate interaction energies, enabling the differentiation between active and inactive conformational states.

## Methodology
- Data Loading: The tool loads MD trajectories for inactive and active states.
- Preprocessing: It slices relevant portions of the trajectories and identifies aromatic residues for further analysis.
### Interaction Calculation:
- Hydrogen Bonds: Calculates hydrogen bond energies based on distance and angle.
- π-π Interactions: Identifies and calculates π-π stacking interactions based on distance.
- Data Aggregation: Compiles interaction energies into a pandas DataFrame, distinguishing between active and inactive states.
### Machine Learning:
- Applies a Random Forest classifier to the interaction data.
- Evaluates model performance using cross-validation.
- Uses SHAP (SHapley Additive exPlanations) to interpret model predictions.

### Result example

<img src="https://github.com/user-attachments/assets/4e34e597-1f4d-46a2-b756-312e25c83efc" alt="image" width="700"/>
