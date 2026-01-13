# Restaurant Visitor EDA (Recruit Restaurant Visitor Forecasting)

## Overview
This mini project explores restaurant visitor traffic patterns using the Kaggle **Recruit Restaurant Visitor Forecasting** dataset.  
The goal is to identify **weekly patterns (day-of-week, weekend effect)** and **monthly trends** and translate them into basic operational insights.

📓 Notebook: [Open in Google Colab](https://colab.research.google.com/github/jiyun040101-maker/restaurant-visitor-eda/blob/main/Recruit_Restaurant_Visitor_Analysis.ipynb)

## Dataset
- Source: Kaggle "Recruit Restaurant Visitor Forecasting"
- File used: `air_visit_data.csv`
- Key columns:
  - `visit_date`: date of restaurant visit
  - `visitors`: number of visitors
  - `air_store_id`: restaurant identifier (for future store-level analysis)

## Key Questions
1. How do average visitors differ by **day of week**?
2. Is there a **weekend effect** (weekend vs weekday)?
3. Do visitor counts vary by **month** (seasonality/trends)?

## Methods
- Converted `visit_date` to datetime
- Feature engineering:
  - `day_of_week` using `.dt.day_name()`
  - `is_weekend` using boolean logic
  - `month` using `.dt.month`
- Aggregation:
  - `groupby` + mean visitors
- Visualization:
  - Bar charts and line charts

## Results (Summary)
- Visitor demand shows clear **weekly patterns** across days of the week.
- Weekend averages differ from weekdays, suggesting a **weekend effect**.
- Monthly averages fluctuate, which may reflect **seasonality, holidays, or promotions**.

## Next Steps
- Store-level analysis using `air_store_id`
- Outlier and variability analysis
- Add holiday/event features

## Tech Stack
- Python (pandas, matplotlib)
- Google Colab
- GitHub

