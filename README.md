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

- ![Data](https://github.com/nzizabenjamin/Uber-Fares-Project/blob/0e52a62ec62a9ca8fb2e3274dba92f3006dc8882/Screenshots/Screenshot%202025-07-27%20051945.png)
- ![Loading in PowerBi](https://github.com/nzizabenjamin/Uber-Fares-Project/blob/0e52a62ec62a9ca8fb2e3274dba92f3006dc8882/Screenshots/Screenshot%202025-07-27%20051931.png)
- ![PowerBi Dashboard](https://github.com/nzizabenjamin/Uber-Fares-Project/blob/ee8c4f72f2697764d62283d158232deae48e4fdd/Screenshots/Screenshot%202025-07-27%20050106.png)

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
| `uber_fares.ipynb` | Python script for data cleaning and feature engineering |
| `Uber_Fare_Analysis.pptx` | Project summary PowerPoint |
| `Uber_Fare.pbix` | Final Power BI dashboard |
| `Screenshots/` | Step-by-step visuals |
| `README.md` | This project documentation |

---

## 🙏 Acknowledgments

- Dataset from Kaggle by Yasser H

---

> “Without data, you're just another person with an opinion.” – W. Edwards Deming
