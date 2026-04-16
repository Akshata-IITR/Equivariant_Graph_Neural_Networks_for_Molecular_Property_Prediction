# Equivariant Graph Neural Networks for Molecular Property Prediction

This project implements **E(n) Equivariant Graph Neural Networks (EGNNs)** to predict the physical and chemical properties of molecules. Unlike standard GNNs, EGNNs are designed to be rotationally and translationally invariant, making them ideal for 3D molecular data where the spatial orientation of atoms is critical.

## Project Overview
Predicting molecular properties is a cornerstone of drug discovery and materials science. This notebook demonstrates:
* Building a custom **EGNN layer** from scratch.
* Processing 3D molecular coordinates and atomic features.
* Training a model to minimize prediction error on benchmark molecular datasets.

## Tech Stack
* **Python**
* **PyTorch / PyTorch Geometric** (Graph Deep Learning)
* **RDKit** (Cheminformatics)
* **Jupyter Notebook**

## Key Features
* **Equivariance:** Ensures that rotating a molecule in 3D space does not change the predicted physical property.
* **Message Passing:** Efficiently aggregates information from neighboring atoms.
* **3D Coordinate Integration:** Uses relative distances between atoms to improve prediction accuracy.

