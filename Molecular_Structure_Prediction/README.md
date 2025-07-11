# Molecular Geometry Prediction

This project presents a hybrid approach to predict and refine the 3D geometries of molecules using a combination of traditional chemical theories, force field methods, and machine learning techniques.

---

## Project Overview

The main goal is to generate realistic molecular structures from SMILES strings by:

1. **Predicting initial geometry using VSEPR theory**
2. **Refining structure with Universal Force Field (UFF)**
3. **Further optimizing geometry using ANI-2x neural network potentials**

This multi-stage pipeline improves molecular geometry prediction for small organic molecules by leveraging domain knowledge and modern ML-based energy calculations.

---

## Pipeline Workflow

The prediction pipeline includes the following stages:

1. **Input SMILES**
2. → **VSEPR-based Initial Geometry**
3. → **UFF Optimization** *(via Open Babel)*
4. → **ANI-2x Refinement** *(via TorchANI)*
5. → **Final 3D Structure + Coordinates**
