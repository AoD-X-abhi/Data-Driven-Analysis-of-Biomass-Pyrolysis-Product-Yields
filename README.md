# PyroYield AI  
**Data-Driven Prediction of Pyrolysis Product Yields Using Ensemble Machine Learning**

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub issues](https://img.shields.io/github/issues/AoD-X-abhi/Data-Driven-Analysis-of-Biomass-Pyrolysis-Product-Yields)](https://github.com/AoD-X-abhi/Data-Driven-Analysis-of-Biomass-Pyrolysis-Product-Yields/issues)
[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.xxxxxx-blue)](https://doi.org/10.5281/zenodo.xxxxxx)

---

## Project Overview

**PyroYield AI** is an end-to-end machine learning framework designed to **predict the product yields (solid, liquid, gas)** from **pyrolysis of biomass and synthetic polymers** using **feedstock composition and process conditions**.

Using **real experimental data**, we train **five state-of-the-art ensemble models**:
- Linear Regression
- Random Forest
- Gradient Boosting
- XGBoost
- LightGBM

**Best performance**: **LightGBM achieves R² = 0.95+ and MAE < 2%** on liquid yield prediction.

---

## What is Pyrolysis?

**Pyrolysis** is the **thermal decomposition of organic materials in the absence of oxygen**, converting complex feedstocks into:
- **Bio-char (solid)**
- **Bio-oil (liquid)**
- **Syngas (gas)**

It is a **key technology** in:
- Bioenergy production
- Waste-to-energy
- Chemical recycling of plastics

---

## Polymers in Focus

We analyze **four major polymers** commonly found in waste streams:

| Polymer | Chemical Formula | Structure |
|--------|------------------|---------|
| **Polyvinyl Chloride (PVC)** | `(C₂H₃Cl)ₙ` | Chlorinated backbone → HCl release during pyrolysis |
| **Polyethylene (PE)** | `(C₂H₄)ₙ` | Simple alkane chain → high liquid yield |
| **Polypropylene (PP)** | `(C₃H₆)ₙ` | Branched structure → wax-like bio-oil |
| **Vinyl Chloride Monomer** | `C₂H₃Cl` | Building block of PVC |

> **Images Explained**:
> - **Left**: 2D structural formula
> - **Right**: 3D ball-and-stick model (Carbon = red, Hydrogen = white, Chlorine = purple)

---

## Key Features

| Feature | Description |
|-------|-----------|
| **Mass Balance Validation** | Ensures `Solid + Liquid + Gas = 100 ± 1.5%` |
| **Feature Engineering** | O/C, H/C, VM/FC ratios, interaction terms |
| **Robust Preprocessing** | Handles `%`, commas, `"N/A"`, missing values |
| **5 ML Models** | Compared with MAE, RMSE, R² |
| **Interactive Visualizations** | Ternary plots, correlation heatmaps |
| **Reproducible** | Conda + pip environments |

---

## Explanation of Images (Add to Report or Slides)

### Image 1: **Vinyl Chloride & Polyvinyl Chloride (PVC)**

![Chemical Structure 1](https://www.google.com/imgres?q=Vinyl%20Chloride%20and%20Polyvinyl%20Chloride%20(PVC)&imgurl=https%3A%2F%2Fwww.shutterstock.com%2Fshutterstock%2Fphotos%2F1021247878%2Fdisplay_1500%2Fstock-vector-polyvinyl-chloride-pvc-and-vinyl-chloride-monomer-molecule-structural-chemical-formula-and-1021247878.jpg&imgrefurl=https%3A%2F%2Fwww.shutterstock.com%2Fimage-vector%2Fpolyvinyl-chloride-pvc-vinyl-monomer-molecule-1021247878&docid=PU2bs8vU0-G_yM&tbnid=V-4Up-HDUwbwjM&vet=12ahUKEwicjZjr3tiQAxVikK8BHf9jHE8QM3oECBwQAA..i&w=1500&h=1426&hcb=2&ved=2ahUKEwicjZjr3tiQAxVikK8BHf9jHE8QM3oECBwQAA)

| Molecule | Formula | Notes |
|--------|--------|-------|
| **Vinyl Chloride** | `C₂H₃Cl` | Monomer; toxic gas |
| **PVC** | `(C₂H₃Cl)ₙ` | Rigid plastic; releases **HCl** during pyrolysis |

> **Pyrolysis Risk**: HCl causes corrosion → needs scrubbing.

---

### Image 2: **Polyethylene (PE) & Polypropylene (PP)**

![Chemical Structure 2](https://www.google.com/imgres?q=Polyethylene%20(PE)%20%26%20Polypropylene%20(PP)&imgurl=https%3A%2F%2Fwww.mdi.org%2Fwp-content%2Fuploads%2F2022%2F04%2FPolyethylene-and-Polypropylene.jpg&imgrefurl=https%3A%2F%2Fwww.mdi.org%2Fblog%2Fpost%2Fwhat-is-the-difference-between-polyethylene-and-polypropylene%2F&docid=83QOvpxLiMzoTM&tbnid=FK6Zk1WN8IMpMM&vet=12ahUKEwj1irPl3tiQAxXUn68BHbUFDoIQM3oECB4QAA..i&w=2048&h=1556&hcb=2&ved=2ahUKEwj1irPl3tiQAxXUn68BHbUFDoIQM3oECB4QAA)

| Polymer | Formula | Notes |
|--------|--------|-------|
| **PE** | `(C₂H₄)ₙ` | High liquid yield (~70–80%) |
| **PP** | `(C₃H₆)ₙ` | Produces waxy bio-oil |

> **Best for Bio-Oil Production**

---

### Image 3: **Polyethylene (Extended Chain)**

![Chemical Structure](https://www.google.com/imgres?q=Polyethylene%20(Extended%20Chain)&imgurl=https%3A%2F%2Fwww.researchgate.net%2Fpublication%2F382238177%2Ffigure%2Ffig1%2FAS%3A11431281272758096%401724241853978%2FSchematic-of-the-chain-extension-process-of-polyethylene-terephthalate-PET-using-SMA.png&imgrefurl=https%3A%2F%2Fwww.researchgate.net%2Ffigure%2FSchematic-of-the-chain-extension-process-of-polyethylene-terephthalate-PET-using-SMA_fig1_382238177&docid=4waZIyj7qtn5BM&tbnid=Z57nuD9ZMM-OsM&vet=12ahUKEwjq47PU3tiQAxX2m68BHUpKDQ4QM3oECBcQAA..i&w=850&h=163&hcb=2&itg=1&ved=2ahUKEwjq47PU3tiQAxX2m68BHUpKDQ4QM3oECBcQAA)

- Shows **long-chain alkane structure**
- Explains **high thermal stability**
- Ideal for **cracking into fuels**
