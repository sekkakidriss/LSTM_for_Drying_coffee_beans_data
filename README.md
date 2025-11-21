# Coffee Drying Prediction Using LSTM Networks

This repository contains a complete workflow for analyzing and predicting coffee bean humidity during the drying process using **LSTM (Long Short-Term Memory) neural networks**.  
The goal is to forecast when the moisture content reaches the target value of **11%**, based on environmental and coffee sensor data collected from multiple regions.

The project includes:

---

##  Project Overview

Coffee drying is a nonlinear time-dependent process influenced by:

- Ambient temperature
- Ambient humidity
- Coffee bean temperature
- Sensor type (DH-200 vs IoT)
- Regional environmental variations

This repository builds a **predictive modeling pipeline** to capture these dynamics and generate accurate forecasts of the humidity level in the **M3 Inferior** section (final drying stage).

---

##  Machine Learning Approach

The workflow uses:

- Multi-region dataset (Genova IoT and Sandona IoT)
- Time-series preprocessing (sliding windows)
- LSTM neural networks with stacked architecture
- 6 activation functions tested:
  - ReLU  
  - Tanh  
  - Sigmoid  
  - SELU  
  - ELU  
  - LeakyReLU

The model performs:

1. **Training** on M1 + M2 sections  
2. **Fitting** a few points from M3  
3. **Predicting** the remaining M3 values  
4. **Evaluating** with MAE, RMSE, and R²

---

##  Included Features

- Data loading, cleaning, and harmonization from Excel
- KDE visualization comparing DH-200 vs IoT sensors
- Summary statistics per region and sensor type
- LSTM model training with validation plots
- M3 prediction visualizations (actual vs fitted vs predicted)
- Performance comparison across activation functions
- Fully documented Jupyter Notebook with Markdown

---

## 📁 Repository Structure


