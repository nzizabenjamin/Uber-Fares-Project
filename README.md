# 🚕 Uber Fares Analysis using Power BI

## 📦 Project Overview

This project explores Uber fare data to uncover insights about pricing patterns, ride demand, time-based trends, and operational factors. The analysis was conducted using Python for preprocessing and Power BI for dashboard visualization.

---

## 📂 Dataset Description

- **Source**: [Uber Fares Dataset on Kaggle](https://www.kaggle.com/datasets/yasserh/uber-fares-dataset)
- **Fields**:
  - `fare_amount` – Amount paid for each ride
  - `pickup_datetime` – Timestamp of ride
  - `pickup_latitude`, `pickup_longitude` – GPS pickup location
  - `dropoff_latitude`, `dropoff_longitude` – GPS dropoff location
  - `passenger_count` – Number of passengers
- **Coverage**: Thousands of rides across New York City

---

## 🧼 Data Cleaning & Preparation

Performed using **Python (Pandas)**:

- Removed nulls, negative fares, and unrealistic passenger counts
- Filtered out invalid geolocations outside NYC bounds
- Converted `pickup_datetime` to datetime format
- Calculated ride distance using geopy
- Engineered new features:
  - `hour`, `day`, `month`, `weekday`
  - `peak_offpeak` time label
- Exported cleaned dataset as `uber_enhanced.csv`

---

## 📊 Key Visualizations (in Power BI)

- 📈 **Fare Distribution**: Histogram and box plot
- ⏱️ **Time-Based Trends**: Rides by hour, weekday, and month
- 🔄 **Peak vs Off-Peak**: Donut chart and stacked column comparison
- 🌍 **Geographic Map**: Pickup distribution across NYC
- 🔥 **Correlation Heatmap**: Relationships between fare, distance, time

---

## 💡 Insights & Outcomes

- Majority of rides cost **$5–$15**
- Rides peak during **7–9 AM** and **5–7 PM**
- **Fridays** are the busiest; **Sundays** are slowest
- **Peak hours account for over 60%** of total rides
- Strong correlation between **distance and fare**

---

## ✅ Recommendations

- Add more drivers during peak hours
- Offer off-peak promotions
- Consider dynamic pricing by hour/day
- Focus marketing around dense pickup zones

---

## 📁 Project Deliverables

| File | Description |
|------|-------------|
| `uber_enhanced.csv` | Cleaned and enriched dataset |
| `uber_analysis.py` | Python script for data cleaning and feature engineering |
| `Uber_Fare_Analysis_Presentation.pptx` | Project summary PowerPoint |
| `Uber_Fare_Analysis.pbix` | Final Power BI dashboard |
| `Screenshots/` | Step-by-step visuals of the dashboard |
| `README.md` | This project documentation |

---

## 🙏 Acknowledgments

- Dataset from Kaggle by Yasser H

---

> “Without data, you're just another person with an opinion.” – W. Edwards Deming
