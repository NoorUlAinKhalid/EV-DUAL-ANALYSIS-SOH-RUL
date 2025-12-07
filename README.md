# Predicting Battery Degradation Trajectories: Evaluating Random Forest and LSTM for Simultaneous SoH and RUL Estimation with Dual Datasets

[![Python 3.x](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

## Project Overview

This repository contains the source code and analysis pipeline for the academic paper titled: **"Predicting Battery Degradation Trajectories: Evaluating Random Forest and LSTM for Simultaneous SoH and RUL Estimation with Dual Datasets."**

The project addresses the critical challenge of accurately forecasting the decline in **Lithium-Ion (Li-ion) battery health** by developing a **dual predictive framework**. This framework simultaneously estimates two key metrics: **State of Health (SoH)** and **Remaining Useful Life (RUL)**.

We perform a rigorous comparison between a **Machine Learning (ML)** approach, specifically **Random Forest (RF)**, and a **Deep Learning (DL)** approach, **Long Short-Term Memory (LSTM)**, to assess their efficacy and generalization capabilities across different data environments.

## Key Contributions & Features

* **Dual-Target Prediction:** Implementation of models capable of predicting both SoH (regression) and RUL (time series) simultaneously.
* **Comparative Analysis:** Head-to-head performance evaluation between Random Forest and LSTM for battery prognostics.
* **Dataset Generalization:** Assessment of model robustness by training and testing on both controlled laboratory data and heterogeneous real-world usage data.
* **Data Preprocessing:** Scripts for normalizing, feature engineering, and preparing raw battery charging/discharging cycle data for both ML and DL architectures.

## Datasets

The study utilizes two distinct datasets to evaluate model performance and generalizability:

1.  **Controlled Laboratory Data:** **NASA PCoE Battery Data**
    * *Source:* Controlled charging/discharging cycles mimicking operating conditions.
    * *Role:* Used for initial training and establishing baseline performance under ideal conditions.
2.  **Real-World Usage Data:** **My Electric Avenue (MEA) Data**
    * *Source:* Data gathered from a fleet of Electric Vehicles (EVs) operating in real-world environments.
    * *Role:* Used to test the model's robustness and generalization to noise and varied usage profiles.

## Models Implemented

| Model                             | Type                  | Target Use Case                      | Key Libraries          |
| :-------------------------------- | :-------------------- | :----------------------------------- | :--------------------- |
| **Random Forest (RF)**            | Machine Learning (ML) | SoH and RUL Regression               | `scikit-learn`         |
| **Long Short-Term Memory (LSTM)** | Deep Learning (DL)    | Time-Series Prediction for RUL & SoH | `TensorFlow` / `Keras` |

### Prerequisites

* Python 3.8+
* `pip` package manager

### Installation

1.  Clone the repository:
    ```bash
    git clone [https://github.com/YourUsername/Battery-SoH-RUL-ML-DL-Comparison.git](https://github.com/YourUsername/Battery-SoH-RUL-ML-DL-Comparison.git)
    cd Battery-SoH-RUL-ML-DL-Comparison
    ```

### Contributions
| Data and implementations | Name         | Email                           | Github Profile  |
| :----------------------- | :----------- | :------------------------------ | :-------------- |
| NASA PCoE                | Faiza Jabbar | fjabbar.msai25seecs@seecs.edu.pk|                 |
| Electric Avenue dataset  | Noor Ul Ain  | nain.msai25seecs@seecs.edu.pk   | NoorUlAinKhalid |
