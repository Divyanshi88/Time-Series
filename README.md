# Time-Series Projects

This repository contains various mini-projects related to **Time Series Analysis and Forecasting**. Each project explores different techniques and models used in time series data analysis, including preprocessing, visualization, trend analysis, and forecasting.

---

### **Mini Project 1: Air Passengers Time Series Analysis**

In this project, we analyze the **Air Passengers** dataset, which contains monthly statistics of international airline passengers from 1949 to 1960. The goal is to explore the trends, seasonality, and patterns in air travel over time using time series analysis techniques.

#### **Key Steps:**

- **Data Preprocessing:**  
  - Convert the **Month** column to a datetime object and set it as the index.  
  - Sort the data chronologically for time series analysis.

- **Visualization:**  
  - Created **Matplotlib line charts** for static visualizations.  
  - Built **interactive time series charts** using Plotly for more engaging exploration.

- **Key Insights:**  
  - Identified seasonal trends and significant growth in the number of passengers over time.  
  - Laid the foundation for advanced forecasting and anomaly detection.

- **Outcome:**  
  This project demonstrates fundamental time series analysis techniques such as data preprocessing and visualization.

---

### **Mini Project 2: Stationarity Analysis of Time Series Data**

In this project, we analyze the stationarity of two time series datasets: **Shampoo Sales Over Time** and **Monthly Beer Production in Australia**. The goal is to determine whether these time series exhibit stationarity and, if not, apply transformations to make them stationary for accurate forecasting.

#### **Key Steps:**

- **Data Preprocessing:**  
  - Downloaded the datasets using the **Kaggle API**.  
  - Loaded the data into **Pandas DataFrames**, checked for missing values, and cleaned the data.

- **Visualization:**  
  - Plotted the datasets to observe trends and seasonality.

- **Stationarity Testing:**  
  - Applied the **Augmented Dickey-Fuller (ADF) Test** to test for stationarity.  
  - Used **differencing** to make the data stationary if necessary.

- **Key Insights:**  
  - Both datasets were **non-stationary**, but after first-order differencing, they became stationary and ready for modeling.

- **Outcome:**  
  This project demonstrates **stationarity analysis** and prepares time series data for predictive modeling techniques like ARIMA.

---

### **Mini Project 3: Wikipedia Page View Time Series Analysis**

In this project, we analyze **Wikipedia page view traffic** to explore trends, seasonality, and stationarity using time series techniques.

#### **Key Steps:**

- **Data Preprocessing:**  
  - Loaded the **Wikipedia page views dataset** into a **Pandas DataFrame**.  
  - Handled **missing values** and converted the date columns into **DateTime format**.

- **Visualization:**  
  - Plotted the **raw time series** and performed **rolling statistics** (mean & standard deviation).  
  - Analyzed dependencies in the data using **Autocorrelation Function (ACF)** plots.

- **Stationarity Testing & Trend Analysis:**  
  - Performed the **Augmented Dickey-Fuller (ADF) Test** for stationarity.  
  - Observed trends and used **seasonal decomposition** to break the series into **trend**, **seasonality**, and **residuals**.

- **Key Insights:**  
  - Identified **seasonality** and **trends** in the data, indicating non-stationarity.  
  - **Weekly seasonality** was found in the data after decomposition.

- **Outcome:**  
  This project provides insights for **future forecasting** by preparing the data for **ARIMA** or other time series forecasting models.

---

### **Mini Project 4: Identifying and Denoising Noise in Electric Production Time Series Data**

In this project, we analyze the **Electric Production time series dataset** to identify and denoise noise, using various filtering techniques to improve data quality and preserve important trends.

#### **Key Steps:**

- **Data Preprocessing:**  
  - Loaded the **Electric Production dataset** using **Pandas**.  
  - Checked for **missing values** and handled them using techniques such as **forward fill** or **interpolation**.  
  - Converted the **date column** into a proper **datetime format** and set it as the index.

- **Noise Identification & Filtering:**  
  - Plotted noise patterns such as **white noise, seasonal noise, and outliers**.  
  - Applied **Moving Average Filter, Exponential Moving Average, Savitzky-Golay Filter, and Butterworth Filters**.

- **Key Insights & Outcome:**  
  - Demonstrated noise reduction techniques to improve forecasting accuracy.

---

### **Mini Project 5: Forecasting Electric Production Using AutoReg Model**

In this project, we apply **AutoReg (Autoregressive) modeling** to forecast **Electric Production** using historical data.

#### **Key Steps:**

- **Data Preprocessing & Stationarity Testing:**  
  - Handled missing values and applied **ADF Test** for stationarity.  
  - Used **differencing** if required.

- **Model Training & Evaluation:**  
  - Used **AutoReg** with lag parameter tuning.  
  - Forecasted future values and evaluated performance using **MSE & RMSE**.

- **Outcome:**  
  - Demonstrated **time series forecasting** using AutoReg and performance evaluation.

---

### **Mini Project 6: ARIMA-based Time Series Forecasting**

In this project, we use the **ARIMA (AutoRegressive Integrated Moving Average) model** to forecast time series data. ARIMA is one of the most powerful statistical models for time series forecasting.

#### **Key Steps:**

- **Data Preprocessing & Stationarity Testing:**  
  - Loaded the dataset and checked for missing values.  
  - Applied **Augmented Dickey-Fuller (ADF) Test** to check stationarity.  
  - Used **differencing** to make the series stationary if necessary.

- **Model Selection & Training:**  
  - Identified optimal **p, d, q** parameters using **ACF/PACF plots**.  
  - Trained the **ARIMA model** on the dataset.

- **Forecasting & Evaluation:**  
  - Forecasted future values using the trained ARIMA model.  
  - Compared predictions with actual values using **RMSE, MSE, and AIC/BIC scores**.

- **Outcome:**  
  - Demonstrated how to use ARIMA for effective time series forecasting and parameter tuning.

---

## **Conclusion**

This repository showcases various aspects of time series analysis and forecasting, from **stationarity testing** to **noise removal and forecasting** using different models such as **AutoReg and ARIMA**. Each project provides a structured approach to analyzing and predicting time series data.

---

Feel free to explore, contribute, or raise issues if you have any suggestions! 🚀

