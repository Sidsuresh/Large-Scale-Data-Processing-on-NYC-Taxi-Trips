# Large-Scale NYC Taxi Data Analytics & ML (1B+ Rows)

This project demonstrates large-scale data engineering and applied machine learning on **1B+ NYC taxi trip records**, using **Apache Spark (PySpark)** on **Databricks**.  
The focus is on **scalable data processing, data quality validation, and feature-driven ML modeling** rather than toy-scale experimentation.

---

## 🚀 Project Overview

The NYC Taxi dataset spans billions of trip records collected over multiple years, making it an ideal benchmark for:
- Distributed data processing
- Schema unification across heterogeneous sources
- Large-scale analytics and ML feature engineering

This project builds an **end-to-end Spark pipeline** from raw ingestion to analytics and regression modeling.


---

## 📊 Dataset

- **Source**: NYC Yellow & Green Taxi Trip Records
- **Scale**: 1B+ rows
- **Time Range**: Multiple years
- **Challenges**:
  - Large file sizes
  - Inconsistent schemas
  - Noisy / unrealistic trip records

---

## 🧹 Data Processing & Validation

Key validation steps applied at scale:
- Removed trips with invalid timestamps, distances, durations, and fares
- Filtered unrealistic speeds and outliers
- Preserved dataset integrity while minimising unnecessary data loss
- Unified schemas across taxi types for consistent downstream analysis

All transformations were implemented using **Spark DataFrame APIs** for distributed execution.

---

## 📈 Analytics & Insights

Using **Spark SQL**, the project explores:
- Temporal demand patterns (hourly, daily, seasonal)
- Spatial trends across pickup and drop-off locations
- Passenger behaviour and tipping patterns
- Revenue distribution across time and geography

Queries are optimised for large-scale execution.

---

## 🤖 Machine Learning

- **Task**: Regression to predict trip total amount
- **Features**: Distance, duration, passenger count, time-based aggregates
- **Models**: scikit-learn regression models trained on Spark-aggregated data
- **Evaluation**: RMSE-based benchmarking against baseline models

This setup reflects **real-world ML pipelines**, where feature engineering and scalability matter more than model novelty.

---

## 🛠️ Tech Stack

- Apache Spark (PySpark)
- Databricks
- Spark SQL
- Python
- scikit-learn

---

## 🎯 Key Takeaways

- Designed scalable pipelines for **billion-row datasets**
- Applied **production-style data validation** at scale
- Demonstrated trade-offs between data quality, performance, and ML accuracy
- Built analytics and ML workflows aligned with real-world data systems

---

## 📌 Notes

This project is intended to showcase **large-scale data engineering and applied ML skills** relevant to Big Tech and data-intensive environments.



