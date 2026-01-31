# Smart Trash: Using Data Analytics for Urban Carbon Reduction ♻️🚛

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![IoT](https://img.shields.io/badge/Focus-Smart%20City-green)
![Sustainability](https://img.shields.io/badge/Impact-Carbon%20Reduction-orange)

## 📌 Project Overview
The **Smart Trash** project optimizes urban waste management using IoT data and predictive analytics. By shifting from fixed schedules to **dynamic collection routes**, we minimize fuel consumption and directly reduce the carbon footprint of sanitation fleets.

## ⚠️ Problem Statement
Traditional waste management systems follow static routes, leading to:
* **High Carbon Emissions:** Trucks visiting empty bins waste diesel and increase $CO_2$.
* **Urban Inefficiency:** Traffic congestion caused by unnecessary garbage truck movement.
* **Environmental Hazard:** Overflowing bins due to lack of real-time monitoring.

## 🎯 Key Objectives
1. **Real-time Monitoring:** Track bin fill levels using simulated IoT sensor data.
2. **Route Optimization:** Implement algorithms to visit only bins above an 80% threshold.
3. **Emission Analysis:** Quantify $CO_2$ savings compared to traditional methods.

## 📊 Dataset Overview
This project utilizes sensor-based datasets containing:
* **Bin_ID:** Unique identifier for each bin.
* **Fill_Level (%):** Real-time capacity data.
* **GPS Coordinates:** Lat/Long for route mapping.
* **Timestamp:** Data used for time-series forecasting.

**Data Source:** [Kaggle Smart Waste Management Dataset](https://www.kaggle.com/datasets/abdalrhmanalramadneh/smart-trash-data)

## 🛠️ Tech Stack & Methodology
* **Language:** Python
* **Data Handling:** `pandas`, `numpy`
* **Optimization:** `scipy` (Spatial Distance Matrices), `Dijkstra's Algorithm`
* **Visualization:** `matplotlib`, `seaborn`

### **The Logic**
The system identifies "Active Bins" (Fill Level > 80%) and calculates the shortest mathematical path between them. It then calculates the **Carbon Impact** using the formula:
$$Saved\ CO_2 = (Baseline\ Distance - Optimized\ Distance) \times Emission\ Factor$$

