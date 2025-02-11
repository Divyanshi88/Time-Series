
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

In this project, we analyze the **Electric Production time series dataset** to identify and denoise noise, using various filtering techniques to improve data quality and preserve important trends. The goal is to manage noise components such as random fluctuations, seasonality, and outliers.

#### **Key Steps:**

1. **Data Loading and Preprocessing:**
   - Loaded the **Electric Production dataset** using **Pandas**.  
   - Checked for **missing values** and handled them using techniques such as **forward fill** or **interpolation**.  
   - Converted the **date column** into a proper **datetime format** and set it as the index for time series analysis.  
   - Plotted the **raw time series** to observe the general patterns, including any evident trends or seasonality.

2. **Identifying Noise in Time Series:**
   - Plotted common types of noise in time series data:
     - **White Noise** (random fluctuations with no correlation)
     - **Seasonal or Cyclical Noise** (periodic, repeating patterns)
     - **Outliers and Irregular Spikes** (extreme or unexpected values)
   - Applied **rolling statistics** (mean & standard deviation) to identify the presence of noise.

3. **Applying Noise Filtering Techniques:**
   - Implemented and compared various denoising methods:
     - **Moving Average Filter (SMA):** Applied with different window sizes and compared the smoothed vs. original time series.
     - **Exponential Moving Average (EMA):** Used a smoothing factor to reduce noise while maintaining trends.
     - **Savitzky-Golay Filter:** Smoothed the time series using **scipy.signal.savgol_filter()**.
     - **Butterworth Filters:** Used **low-pass**, **high-pass**, and **band-pass filters** to remove different types of noise.

4. **Evaluating the Denoising Performance:**
   - Compared the filters by:
     - Plotting the **original** vs. **filtered time series**.
     - Measuring **Mean Squared Error (MSE)** or **Signal-to-Noise Ratio (SNR)** before and after filtering.

5. **Insights and Conclusion:**
   - Different filters were effective in reducing noise:
     - **Low-pass filters** effectively removed short-term fluctuations.
     - **High-pass filters** preserved seasonal variations by removing long-term trends.
   - These techniques helped enhance the time series data for further analysis and forecasting.

---

## **Conclusion**

This repository showcases various aspects of time series analysis and forecasting, from **stationarity testing** to **noise removal**. Each mini-project demonstrates critical techniques that can be used to process and model time series data for forecasting and anomaly detection tasks.
