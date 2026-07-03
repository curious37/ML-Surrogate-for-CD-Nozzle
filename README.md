# Machine Learning-Based Surrogate Modeling of Supersonic Nozzle Flows

## Overview

This repository contains the Python implementation developed for the M.Tech dissertation titled:

**"Machine Learning-Based Surrogate Modeling of Supersonic Nozzle Flows Using CFD-Generated Data."**

The objective of this work is to develop machine learning surrogate models capable of predicting the centerline Mach number distribution in convergent-divergent nozzles with varying exit diameters and nozzle pressure ratios.

---

## Repository Contents

- `dataset.py` – Dataset generation, preprocessing, normalization, and shock-aware weighting.
- `train_fcnn.py` – Baseline Fully Connected Neural Network (FCNN).
- `train_residual.py` – Residual Multi-Layer Perceptron (Residual MLP).
- `train_weighted_residual.py` – Shock-Weighted Residual MLP.

---

## Input Features

- Normalized axial location (`x_norm`)
- Normalized area ratio (`AeAt_norm`)
- Normalized nozzle pressure ratio (`NPRr_norm`)

## Output

- Normalized Mach number (`Mach_norm`)

---

## Machine Learning Models

- Fully Connected Neural Network (FCNN)
- Residual Multi-Layer Perceptron (Residual MLP)
- Shock-Weighted Residual MLP

---

## Software Used

- Python
- PyTorch
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- SciPy

---

## How to Run

### Step 1

Install the required packages:

```bash
pip install -r requirements.txt
```

### Step 2

check the datasets:

### Step 3

Train the models:

```bash
python train_fcnn.py
```

```bash
python train_residual.py
```

```bash
python train_weighted_residual.py
```

---

## Author

**Mukund Singh**

M.Tech in Jet Propulsion and Gas Turbine Plant

The Maharaja Sayajirao University of Baroda

---

This repository accompanies the M.Tech dissertation and is intended for academic and research purposes.
