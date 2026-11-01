[github_readme.md](https://github.com/user-attachments/files/34229113/github_readme.md)
# Diwali AirGuard 🎇🌫️

> **From pollution prediction to pollution prevention**  
> An AI platform that helps cities anticipate pollution, protect exposed populations, and evaluate what interventions actually work.

---

## 📌 Table of Contents
- [Overview](#-overview)
- [The Problem & The Solution](#-the-problem--the-solution)
- [Key Features Across the Festival Cycle](#-key-features-across-the-festival-cycle)
- [Technical Architecture & AI Engine](#-technical-architecture--ai-engine)
- [Tech Stack](#-tech-stack)
- [Project Roadmap](#-project-roadmap)
- [Metrics & Evaluation](#-metrics--evaluation)
- [Impact & Benefits](#-impact--benefits)
- [Why Diwali AirGuard?](#-why-diwali-airguard)

---

## 🎆 Overview

During major festival periods like Diwali, urban areas experience extreme spikes in air pollution ($PM_{2.5}$ and $PM_{10}$). Most existing platforms only report post-event Air Quality Index (AQI) values, leaving cities reacting to pollution rather than preventing exposure.

**Diwali AirGuard** bridges this gap by offering an end-to-end AI platform. It transitions municipal authorities, residents, and researchers from reactive monitoring to proactive management, live incident response, and empirical impact evaluation. While optimized for festival pollution cycles, **Diwali AirGuard runs year-round**.

---

## 🎯 The Problem & The Solution

### The Gap Today
* **Where** will air quality reach dangerous levels *before* it happens?
* **Which** specific neighbourhoods and vulnerable populations need help first?
* **Which** interventions (sweeping, water sprinkling, traffic rerouting) actually work?

### The AirGuard Approach
Diwali AirGuard addresses the entire festival pollution cycle in three distinct phases:

```
[ BEFORE ] ---> Predict & Prepare (Hotspots & Forecasts)
[ DURING ] ---> Detect & Respond (Live Incidents & Safe Routes)
[ AFTER  ] ---> Verify & Improve (Intervention Checks & Resilience Scores)
```

---

## 🚀 Key Features Across the Festival Cycle

### 1. BEFORE: Predict & Prepare
* **Neighbourhood Forecasts:** Anticipate $PM_{2.5}$ and $PM_{10}$ levels ahead of time using historical and weather data.
* **Hotspot Identification & Exposure Ranking:** Identify high-risk zones based on predicted pollution combined with population density and sensitive site locations (hospitals, schools).

### 2. DURING: Detect & Respond
* **Live Incident Detection:** Real-time anomaly detection to flag severe, localized spikes as they happen.
* **Exposure Reduction Routing:** Suggest safer, lower-exposure routes for residents and alert vulnerable populations.
* **Priority Views for Authorities:** Help municipal teams allocate resources efficiently (e.g., smog towers, anti-smog guns, traffic diversions).

### 3. AFTER: Verify & Improve
* **Intervention Impact Assessment:** Statistically verify the effectiveness of municipal actions by comparing intervention zones with similar baseline control zones.
* **Recovery Tracking & Resilience Scores:** Measure the time required for neighbourhood air quality to return to normal baseline levels post-festival.

---

## 🛠️ Technical Architecture & AI Engine

The platform operates on a clear pipeline: **Data In $\rightarrow$ AI Engine $\rightarrow$ Action Out**.

```
+-----------------------------------+
|             DATA IN               |
| - Historical & Live Air Quality   |
| - Weather Forecasts               |
| - Maps & Road Networks            |
| - Population & Sensitive Sites    |
| - Past Episodes & Interventions   |
+-----------------------------------+
                  |
                  v
+-----------------------------------+       +-----------------------------------+
|            AI ENGINE              |       |            ACTION OUT             |
| 1. Forecasting:                   |       | - Residents:                      |
|    Random Forest Regressor        | ----> |   Alerts & low-exposure routes    |
|    (Baseline: Linear Regression)  |       |                                   |
| 2. Area Estimation:               |       | - Authorities:                    |
|    K-Nearest Neighbours (KNN)     | ----> |   Priority maps & action plans    |
| 3. Incident Detection:            |       |                                   |
|    Rolling Z-Score &              | ----> | - Researchers:                    |
|    Isolation Forest               |       |   Recovery tracking & evidence    |
| 4. Exposure Ranking:              |       |                                   |
|    Risk Score + K-Means           |       +-----------------------------------+
| 5. Intervention Check:            |
|    Difference-in-Differences      |
|    (Linear Reg + SciPy t-test)    |
+-----------------------------------+
```

---

## 🧰 Tech Stack

Built using a lightweight, beginner-friendly Python toolkit:

| Layer / Category | Tools & Libraries |
| :--- | :--- |
| **Data Processing** | `pandas`, `NumPy` |
| **Machine Learning & Stats** | `scikit-learn`, `SciPy` |
| **Spatial & Mapping** | `GeoPandas`, `Folium` |
| **Visualization** | `Matplotlib`, `Seaborn` |
| **Dashboard & UI** | `Streamlit` |

---

## 🛣️ Project Roadmap

* **Stage 1: Forecast**
  * Train $PM_{2.5}$ / $PM_{10}$ forecasting models on historical air quality and weather data.
* **Stage 2: Detect**
  * Integrate live data streams, anomaly detection algorithms, and spatial exposure ranking.
* **Stage 3: Respond**
  * Implement real-time notifications for residents and dedicated priority dashboards for city officials.
* **Stage 4: Evaluate**
  * Deploy post-event Difference-in-Differences evaluation, recovery tracking, and year-round continuous monitoring.

---

## 📊 Metrics & Evaluation

| Component | Metric / Evaluation Method |
| :--- | :--- |
| **Forecasting** | Mean Absolute Error ($MAE$), Root Mean Squared Error ($RMSE$) |
| **Incident Detection** | Precision, Recall, Detection Delay |
| **Area Estimation** | Interpolation Error, Uncertainty Calibration |
| **Prioritization** | Population Coverage in High-Risk Zones |
| **Interventions** | Difference-in-Differences (Treatment vs. Control Baseline) |
| **Recovery** | Time to Return to Normal Baseline ($T_{recovery}$) |

---

## 💡 Impacts & Benefits

* **For Residents:** Receive early warnings and lower-exposure navigation routes to reduce personal health risks.
* **For Municipal Authorities:** Target deployment of anti-smog equipment, water sprinklers, and traffic control teams to high-priority zones based on data.
* **For Researchers & Policy Makers:** Access rigorous statistical evidence on which interventions deliver measurable improvements and how quickly areas recover.

---

## ⚡ Why Diwali AirGuard?

| Feature | Conventional AQI Platform | Diwali AirGuard |
| :--- | :---: | :---: |
| **Approach** | Reports current pollution | Predicts & detects incidents proactively |
| **Coverage** | Limited to station locations | Estimates air quality in under-monitored gaps |
| **Alerts** | Generic broadcast warnings | Ranks areas by population exposure risk |
| **Actionability** | Displays raw trends | Recommends targeted, localized action |
| **Lifecycle** | Stops at reporting/forecasting | Evaluates intervention impact & tracks recovery |

---

## 👥 Team
**Team Name:** Nexgen 
**Members:** Raizel Chauhan
             Harpreet Singh 
             Ashmit Mittal 
             Bhavika Ghai 

---
*Diwali AirGuard — Moving cities from reacting to pollution to anticipating, managing, and learning from it.*
