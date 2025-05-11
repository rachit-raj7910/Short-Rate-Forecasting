# Short Rate Forecasting

This repository contains a comparative study of **short-term interest rate forecasting** using both classical stochastic models and modern machine learning techniques. The focus is on modeling **13-week U.S. Treasury Bill rates**, evaluated through a **rolling window** approach and benchmarked against a **Random Walk**.

---

##  Objective

To evaluate the forecasting performance of:
- **Vasicek Model**
- **Cox-Ingersoll-Ross (CIR) Model**
- **Random Forest Regressor**
- **Long Short-Term Memory (LSTM)**

Against a **Random Walk baseline** across multiple horizons:
- **1 day**
- **1 week**
- **1 month**
- **3 months**

---

## Models

###  Mathematical Finance
- **Vasicek Model** – a mean-reverting process with constant volatility.
- **CIR Model** – ensures non-negative rates with state-dependent volatility.

###  Machine Learning
- **Random Forest** – captures nonlinear dependencies using ensemble decision trees.
- **LSTM** – a type of RNN capable of learning time-dependent patterns.

---

##  Methodology

All models use a **rolling window approach** with:
- **90 observations per training step**
- Forecasts made for **1, 7, 30, and 90 steps ahead**

---

## Evaluation Metrics

- **Mean Squared Error (MSE)** – for accuracy
- **Directional Accuracy** – for predicting rate movement direction
- **Visual Forecast Plots** – for interpretability

---

##  Repository Structure

| File                                | Description                                                             |
|-------------------------------------|-------------------------------------------------------------------------|
| `Short_Forecasting_Rate_.ipynb`     | Main notebook comparing all models using rolling windows               |
| `CIR_Simulation_and_Estimation_.ipynb` | Simulation + calibration of CIR model using MLE                         |
| `Vasicek_Simulation_and_Estimation_.ipynb` | Simulation + calibration of Vasicek model using MLE                      |
| `treasury_bill_data.xlsx`           | Historical 13-week U.S. Treasury Bill data                              |

---





