# Time-Series
This repository contains various mini-projects related to Time Series Analysis and Forecasting. Each project explores different techniques and models used in time series data analysis, including preprocessing, visualization, trend analysis, and forecasting.




### **Mini Project 1: Air Passengers Time Series Analysis**
In this project, we analyze the Air Passengers dataset, which contains monthly statistics of international airline passengers from 1949 to 1960. The goal is to explore the trends, seasonality, and patterns in air travel over time using time series analysis techniques.
---
### **Key Steps:**
#### **Data Preprocessing:**

Convert the Month column to a datetime object and set it as the index.
Sort the data chronologically to prepare for time series analysis.
Visualization:

We create Matplotlib line charts for static visualizations.
Interactive time series charts are built using Plotly, allowing us to explore the data more interactively.
Key Insights:

By visualizing the number of passengers over time, we can identify seasonal trends and significant growth over the years.
This project lays the groundwork for more advanced time series forecasting and anomaly detection in future mini-projects.
Outcome:
This project serves as a foundational example of time series analysis, demonstrating data preprocessing and visualization techniques that can be applied to various time series datasets.
---
### **Mini Project 2: Stationarity Analysis of Time Series Data**  

In this project, we analyze the stationarity of two time series datasets: **Shampoo Sales Over Time** and **Monthly Beer Production in Australia**. The goal is to determine whether these time series exhibit stationarity and, if not, apply transformations to make them stationary, which is essential for accurate forecasting.

---

### **Key Steps:**  

#### **1. Data Preprocessing:**  
- Downloaded **time series datasets** from Kaggle using the Kaggle API.  
- Loaded the datasets into Pandas DataFrames for analysis.  
- Checked and cleaned the data by handling missing values and ensuring proper formatting.  

#### **2. Visualization:**  
- Plotted **Shampoo Sales Over Time** and **Monthly Beer Production** using Matplotlib to observe trends and seasonality.  
- Identified upward trends in both datasets, indicating potential non-stationarity.  

#### **3. Stationarity Testing:**  
- Applied the **Augmented Dickey-Fuller (ADF) Test** to assess whether the time series is stationary.  
- Interpreted ADF statistics and **p-values** to determine stationarity.  
- If the series was non-stationary, applied **differencing** to remove trends and re-tested using the ADF test.  

#### **4. Key Insights:**  
- Both datasets were initially **non-stationary**, as indicated by high p-values in the ADF test.  
- After **first-order differencing**, both time series became stationary, meaning they could now be used for further time series modeling and forecasting.  

---

### **Outcome:**  
This project demonstrates **stationarity analysis**, an essential step in time series forecasting. By identifying and transforming non-stationary data into a stationary format, we prepare it for **ARIMA and other predictive modeling techniques** in future mini-projects.
## **Mini Project: Wikipedia Page View Time Series Analysis**  

In this project, we analyze **Wikipedia page view traffic** using time series techniques to explore trends, seasonality, and stationarity. The goal is to understand the underlying patterns in the data and prepare it for future forecasting.  

### **Key Steps:**  

#### **1. Data Preprocessing:**  
- Loaded the **Wikipedia page views dataset** into a Pandas DataFrame.  
- Checked for **missing values** and handled them using **forward fill (ffill)** to ensure continuity.  
- Converted the date columns into **DateTime format** and set the index for time series analysis.  

#### **2. Visualization:**  
- Plotted the **raw time series** to observe the overall trends in Wikipedia traffic.  
- Applied **rolling statistics (mean & standard deviation)** to analyze changes over time.  
- Used **Autocorrelation Function (ACF) plots** to understand dependencies in the time series.  

#### **3. Stationarity Testing & Trend Analysis:**  
- Conducted an **Augmented Dickey-Fuller (ADF) Test** to check stationarity.  
- Observed **non-stationary behavior** in the data, indicating trends and seasonality.  
- Used **seasonal decomposition** (additive model) to break the series into **trend, seasonality, and residuals** for better interpretation.  

#### **4. Key Insights:**  
- The **Wikipedia page views dataset** showed **strong seasonality and trends**, leading to non-stationarity.  
- Rolling mean analysis indicated **long-term variations in page views**.  
- After decomposing the series, **weekly seasonality** was observed, suggesting periodic fluctuations in traffic.  
- These insights help in **future forecasting** by preparing the data for further modeling using ARIMA or other predictive techniques.  

---

