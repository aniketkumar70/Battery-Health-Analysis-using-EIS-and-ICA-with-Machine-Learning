# Battery Health Analysis using EIS and ICA with Machine Learning

## Overview

This project explores battery degradation using Electrochemical Impedance Spectroscopy (EIS) and Incremental Capacity Analysis (ICA). The dataset consists of lithium-ion batteries cycled through various operational profiles (charge, discharge, and EIS measurements) at different temperatures. The goal is to analyze aging behavior and develop predictive models for battery health indicators such as capacity and remaining useful life (RUL).

---

## Dataset Description

- The dataset contains multiple batches of experiments.
- Each battery cell was cycled until it reached end-of-life (EOL).
- EIS measurements were taken at different aging stages.
- Charge/discharge cycle data is also provided.
- Data is stored in `.mat` format with detailed experiment metadata.

---
  ## Data Source

The dataset can be found on Kaggle:

🔗 [Battery Aging and EIS Dataset on Kaggle](https://www.kaggle.com/datasets/interacts/anticithhealthdataset)

*Note: Make sure you are logged into your Kaggle account to download the dataset.*


---

## Objectives

### a) EIS-Based 3D Visualization

Create a 3D plot showing how impedance evolves with aging:
- **X-axis**: Real part of impedance (Z')
- **Y-axis**: Imaginary part of impedance (Z'')
- **Z-axis**: Cycle count (aging)

Assume temperature and other environmental conditions are constant.

### b) Incremental Capacity Analysis (ICA)

- From typical charge/discharge cycle data, derive ICA plots showing **dQ/dV vs Voltage**.
- Visualize how ICA peaks shift over time with aging in a 3D plot:
  - **X-axis**: dQ/dV
  - **Y-axis**: Voltage
  - **Z-axis**: Cycle count

This analysis reveals how the battery's internal electrochemical behavior changes.

### c) Machine Learning Model

Build and evaluate a machine learning model to:
- Predict **current battery capacity** from EIS data.
- Explore features like impedance spectrum, cycle count, etc.
- Train, validate, and test your model on relevant portions of the dataset.

---


## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/battery-health-eis-ica.git
   cd battery-health-eis-ica

