# NTT-Stock-Price-Prediction-with-LSTM

## Overview of the Time Series Forecasting Model for NTT Stock Prices

In this project, I developed a time series forecasting model using NTT stock price data. The process began with exploratory data analysis (EDA) to uncover trends, seasonality, and data distribution. I then applied a Long Short-Term Memory (LSTM) neural network to capture temporal dependencies crucial for accurate stock price forecasting.

The data underwent comprehensive preprocessing, including handling missing values, feature scaling, and the creation of new features like moving averages and lagged values. Among various models evaluated, the LSTM demonstrated effective forecasting with a Root Mean Squared Error (RMSE) of **3.09**, forecasting a 30-day downward trend from **178.97** to **102.04**. This project highlights the ability of LSTM to model complex, nonlinear dynamics in financial time series.

---

##  Task Content

### 1. Read and Analyze the Data

**Overview:**
Imported necessary libraries and explored the NTT stock price dataset. Conducted statistical summary analysis, checked for missing values, trends, and seasonality, and identified potential outliers.

---

### 2. Data Visualization

**Overview:**
Utilized Seaborn and Matplotlib to generate visualizations, including correlation heatmaps and histograms, to understand relationships between features and their distributions.

---

### 3. Data Preprocessing and Feature Engineering

**Overview:**
Applied preprocessing steps such as imputing missing values, scaling features, and creating new time-based variables (e.g., moving averages, lagged returns). These enhancements improved learning patterns and model accuracy.

---

### 4. Model Selection and Training

**Overview:**
Implemented traditional regression models (Linear Regression, Random Forest, CatBoost, Gradient Boosting, etc.) alongside LSTM.
LSTM was chosen for time series forecasting due to its strength in capturing sequential patterns and long-term dependencies. The model achieved convergence across 10 epochs, reducing training loss from **7.01e-04** to **1.01e-04**, showing strong learning behavior.

---

### 5. Model Evaluation and Results

**Regression Model Performance (R² Scores):**

* Linear Regression: **95.46%**
* Gradient Boosting: **95.05%**
* CatBoost: **94.97%**
* Random Forest: **94.67%**
* AdaBoost: **94.78%**
* K-Neighbors Regressor: **93.80%**
* Decision Tree: **93.74%**
* Support Vector Regressor: **93.59%**

**Sample Predictions for First 5 Days (from selected models):**

* Linear Regression: \[1.82, 21.94, 18.97, 16.32, 6.55]
* Random Forest: \[2.63, 23.97, 17.88, 16.24, 6.29]
* CatBoost: \[2.33, 23.53, 18.39, 16.73, 6.20]

**LSTM Forecast:**

* RMSE: **3.09**
* 30-day trend: From **178.97** → **102.04**

---

### 6. Conclusion

This project demonstrates the comparative strength of both traditional ML regression models and deep learning for stock forecasting.

* **Linear Regression** delivered the highest R² (95.46%) among classical models.
* **LSTM** effectively forecasted a downward trend in NTT stock prices, proving useful in time-dependent financial prediction.
* LSTM’s performance and convergence indicate strong generalization on sequential stock data.
