# Enhancing Graph Neural Networks for Molecular Property Prediction Using Lie Symmetry and Cromatic Invariants

This project implements **E(n) Equivariant Graph Neural Networks (EGNNs)** and **Graph coloring** to predict the properties of molecules. 
Unlike standard GNNs, EGNNs are designed to be rotationally and translationally invariant, making them ideal for 3D molecular data where the spatial orientation of atoms is critical. Adding Graph Coloring to this model our new model also works for strerioisomers.
As for Strerioisomers GNN and EGNN both are incapable of predicting properties. LieColorGNN will assign unique color to each node using 2-distance coloring and after using that unique color as a new feature we can clear confusion of GNN and EGNN for assuming strerioisomers exactly same molecule and predicting same property for both isomers.

## Project Overview
Predicting molecular properties is a cornerstone of drug discovery and materials science. This notebook demonstrates:
* Building a custom **EGNN layer** from scratch.
* Processing 3D molecular coordinates and atomic features.
* Using graph coloring for unique color for each molecule
* Training a model to minimize prediction error on benchmark molecular datasets.

## Tech Stack
* **Python**
* **PyTorch / PyTorch Geometric** 
* **Jupyter Notebook**

## Key Features
* **Equivariance:** Ensures that rotating a molecule in 3D space does not change the predicted physical property.
* **Chromatic Invariance:** Ensures we get different coloring for strerioisomers as they both can have different properties
* **Message Passing:** Efficiently aggregates information from neighboring atoms.
* **3D Coordinate Integration:** Uses relative distances between atoms to improve prediction accuracy.



