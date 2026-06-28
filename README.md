# Hybrid DCA-LSTM Framework for Oil Well Production Forecasting

This repository contains the official implementation accompanying the manuscript:

> **"A Hybrid Physics-Informed Deep Learning Framework for Oil Well Production Forecasting: Integrating Arps Decline Curve Analysis with Long Short-Term Memory Networks"**

### Authors
* **Stephen Ebuka Iheagwara**
* **Adefisan Peace Folashade**
* **Oluwaseyi Ezekiel Olorunshola**
* **Henry Onyeoma Mafua**

---

## 📌 Project Overview
This framework introduces a hybrid physics-informed machine learning approach to improve the accuracy and reliability of oil well production forecasting. By integrating the physical domain knowledge of **Arps Decline Curve Analysis (DCA)** with the sequential pattern-learning capabilities of **Long Short-Term Memory (LSTM)** networks, this architecture mitigates data scarcity issues and ensures physically consistent forecasts.

---

## 📊 Manuscript Figures & Visualizations
The repository includes the core figures discussed in the manuscript. Additional technical charts can be generated dynamically by executing the repository notebooks.

### 📈 Fig. 1: Raw Production Data
* **Manuscript Context:** §3.1 Dataset analysis
* **Description:** Baseline historical production profile from the Volve field.
![Fig. 1 Raw Production](figures/fig1_raw_production.png) *(Note: Update file extension/name if different)*

### 📉 Fig. 2: Arps DCA Curve Fitting
* **Manuscript Context:** §4.1 DCA empirical results
* **Description:** Empirical Decline Curve Analysis parameters fitted to setting historical constraints.
![Fig. 2 DCA Fit](figures/fig2_dca_fit.png)

### 📊 Fig. 3: Training Loss Convergence
* **Manuscript Context:** §4.2 LSTM network optimization training phase
* **Description:** Training and validation loss trajectory showing model convergence.
![Fig. 3 Loss Curve](figures/fig3_loss_curve.png)

### 🔍 Fig. 4: Residual Error Distribution
* **Manuscript Context:** §4.2 LSTM training analysis
* **Description:** Visual error variance tracking showing network deviation patterns.
![Fig. 4 Residuals](figures/fig4_residuals.png)

### 🔮 Fig. 5: Comparative Forecast Performance
* **Manuscript Context:** §4.4 Comparative evaluation summary
* **Description:** Side-by-side performance matching baseline models against the hybrid framework.
![Fig. 5 Forecast Comparison](figures/fig5_forecast_comparison.png)

---

## 📁 Repository Structure

```text
├── data/
│   ├── sample_data.csv          # Subset of data for testing execution
│   └── download_instructions.md # Steps to download the full Volve dataset
├── figures/
│   ├── fig1_raw_production.png  # Historical raw production plots
│   ├── fig2_dca_fit.png         # Arps decline fitting charts
│   ├── fig3_loss_curve.png      # Training/validation optimization plots
│   ├── fig4_residuals.png       # Error variance distributions
│   └── fig5_forecast_comparison.png # Comparative framework forecasts
├── notebooks/
│   ├── 1_data_preprocessing.ipynb
│   ├── 2_arps_dca_fitting.ipynb
│   ├── 3_hybrid_dca_lstm_training.ipynb
│   └── 4_evaluation.ipynb
└── README.md
```

---

## 💾 Dataset Access
The model is validated using open-source production data from the **Equinor Volve Field**. 
* **Source:** Access the dataset via the official [Databricks Marketplace Volve Data Village](https://databricks.com) profile.
* For complete local setup instructions, see the guide inside the `data/download_instructions.md` file.

---

## 🚀 Getting Started & Replication

### 1. Clone the Repository
```bash
git clone https://github.com
cd YOUR_REPOSITORY_NAME
```

### 2. Environment Setup
Ensure you have Jupyter installed alongside standard scientific computing packages (`numpy`, `pandas`, `scikit-learn`, `tensorflow`/`pytorch`, `matplotlib`).

### 3. Workflow Execution Order
To reproduce the manuscript findings, execute the clean notebooks in the following sequential order:
1. **`1_data_preprocessing.ipynb`**: Handles parsing, cleaning, and formatting the raw Volve production metrics.
2. **`2_arps_dca_fitting.ipynb`**: Fits empirical Arps physics parameters to set historical baseline constraints.
3. **`3_hybrid_dca_lstm_training.ipynb`**: Combines physics-derived DCA constraints into the neural network framework.
4. **`4_evaluation.ipynb`**: Generates performance charts, calculates error metrics, and outputs the project figures.
