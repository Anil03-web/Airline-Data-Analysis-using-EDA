# ✈️ Airline Flight Price Analysis

A comprehensive Exploratory Data Analysis (EDA) project aimed at understanding patterns in flight ticket prices across major Indian airlines. This project identifies how factors like airline type, number of stops, duration, departure/arrival times, and days left before departure influence ticket prices.

---

## 📌 Project Overview

This project analyzes a dataset containing over **300K+ flight records**, followed by:

- Data cleaning & preprocessing  
- Handling missing values, duplicates, and outliers  
- Univariate, bivariate, and multivariate analysis  
- Deriving insights on pricing, routes, duration, and airline operations  

The **target variable** in this dataset is `price`.

---

## 📂 Dataset Information

- **Rows:** 300K+  
- **Columns:** 12  
- **Key features:**  
  - `airline`  
  - `source_city`, `destination_city`  
  - `stops`  
  - `departure_time`, `arrival_time`  
  - `duration`  
  - `days_left`  
  - `price`

---

## 🧹 Data Cleaning Summary

### ✔ Handling Missing Values
- Filled categorical nulls using **mode**
- Filled numerical nulls (`duration`, `price`) using **median**
- Median avoids distortion from outliers

### ✔ Duplicate Removal
- Found 6000+ duplicates → removed

### ✔ Outlier Treatment
- Used **IQR method**  
- Outliers mainly in duration & price  
- Removed values outside defined lower & upper fence

---

## 🔍 Exploratory Data Analysis (EDA)

### 📊 Univariate Insights
- **Vistara** operates the highest number of flights  
- Most flights are **one-stop**  
- Majority ticket prices fall between **₹1,000–₹15,000**  
- AirAsia offers the **cheapest average fares**

### 🔗 Bivariate Insights
- Zero-stop flights are **cheapest and shortest**
- Business class fares are significantly higher  
- Very weak negative correlation between **days_left** and **price**  
- Prices slightly increase as departure date approaches

### 🔀 Multivariate Insights
- Longest average durations appear on **Kolkata ↔ Chennai** routes  
- Shortest average durations: **Mumbai → Delhi**, **Bangalore → Delhi**  
- Vistara & Air India provide both **Business & Economy** classes  

---

## ⭐ Key Findings

### ✈ Airline-Level Insights
- Vistara dominates in number of flights and highest price range
- AirAsia is the most cost-effective airline
- Indigo offers the **shortest average flight durations**

### 🛑 Stops vs Price
- **Zero stops = lowest price**
- **One-stop flights = costliest**
- Flights with two or more stops show competitive pricing

### 🕒 Time-Based Patterns
- Most departures occur in **Morning**
- Most arrivals occur at **Night**
- Late-Night departures tend to be cheaper

### 🧭 Route Insights
- Cheapest routes:  
  - Chennai → Hyderabad  
  - Chennai → Bangalore  
- Longest avg durations:  
  - Kolkata ↔ Chennai

---

## 🛠 Technologies Used

- **Python**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**
- **Jupyter Notebook**

---

