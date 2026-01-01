Here’s a **clean, professional README.md** you can directly use for your project (IEEE / academic-style friendly). You can paste this as-is into a `README.md` file.

---

# Household Power Consumption Forecasting Using Time Series and Machine Learning Models

##  Project Overview

This project focuses on **forecasting household electricity consumption** using a combination of **classical time-series models**, **machine learning regressors**, and **deep learning architectures**. Accurate energy demand forecasting is crucial for smart grid management, energy planning, and efficient resource utilization.

I evaluated and compare multiple forecasting approaches on historical household power consumption data to analyze their prediction accuracy, stability, and real-world applicability.

---

##  Dataset Description

* **Dataset:** Household Power Consumption Dataset
* **Source:** UCI Machine Learning Repository
* **Target Variable:** `Global_active_power` (kilowatt)
* **Time Resolution:** Minute-level data aggregated to **daily average consumption**
* **Preprocessing Steps:**

  * Date–time parsing and indexing
  * Handling missing values using forward fill
  * Resampling to daily frequency
  * Train–test split (80% training, 20% testing)

---

##  Models Implemented

The project evaluates three different modeling paradigms:

### 1️ Classical Time-Series Model

* **SARIMA (Seasonal ARIMA)**

  * Captures trend and weekly seasonality
  * Suitable for linear and seasonal patterns

### 2️ Machine Learning Model

* **Random Forest Regressor**

  * Uses lag-based supervised features
  * Handles non-linear relationships effectively

### 3️ Deep Learning Model

* **LSTM (Long Short-Term Memory)**

  * Sequence-based learning with temporal dependencies
  * Effective for capturing long-term patterns in time series data

---

##  Evaluation Metrics

Model performance is evaluated using standard forecasting error metrics:

* **MAE (Mean Absolute Error)**
* **RMSE (Root Mean Squared Error)**
* **MAPE (Mean Absolute Percentage Error)**

These metrics provide insights into absolute accuracy, variance of errors, and relative percentage deviation.

---

##  Visualization

The following visualizations are generated for analysis and comparison:

* Time-series plots of **actual vs predicted values**
* Training vs validation loss curves (LSTM)
* **Bar chart comparison of MAE, RMSE, and MAPE** across models


---

## 🏆 Results Summary

| Model         | MAE    | RMSE   | MAPE (%) |
| ------------- | ------ | ------ | -------- |
| SARIMA        | 1.0473 | 1.1363 | 144.47   |
| Random Forest | 0.1827 | 0.2449 | 23.48    |
| LSTM          | 0.1866 | 0.2504 | 25.34    |

**Key Observation:**
Random Forest and LSTM significantly outperform SARIMA, with Random Forest achieving the best overall accuracy on this dataset.

---

##  Future Work

Future extensions of this project may include incorporating exogenous variables such as temperature and occupancy, exploring advanced deep learning architectures like GRU and Seq2Seq models, applying probabilistic forecasting techniques for uncertainty estimation, and deploying the models in real-time smart grid environments.

---

##  Technologies Used

* Python
* Pandas, NumPy
* Matplotlib
* Statsmodels
* Scikit-learn
* TensorFlow / Keras

---

##  Project Structure

```
├── data/
│   └── household_power_consumption.txt
├── notebooks/
│   └── mlfinal.ipynb
├── README.md
```

---

##  License

This project is intended for **academic and research purposes only**.

