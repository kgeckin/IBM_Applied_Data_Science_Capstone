# 🚀 SpaceX Falcon 9 First Stage Landing Prediction

## Final presentation

The original IBM / Coursera 47-slide template has been completed with code evidence, SQL outputs, visualizations and linked notebooks. The files are staged for upload.

**[Module 5 presentation and evidence guide](Module5/README.md)**

## Outline

- [Summary](#summary)
- [Introduction](#introduction)
- [Methodology](#methodology)
- [Results](#results)
- [Conclusion](#conclusion)
- [Appendix & References](#appendix--references)

---

## Summary

This project is the capstone for the IBM Data Science Professional Certificate. The aim is to predict whether the Falcon 9 first stage will successfully land, helping both SpaceX and potential competitors to optimize launch operations and costs.

- **Data Sources:**  
  SpaceX public API, Wikipedia, and course-provided CSV files.
- **Data Wrangling:**  
  Collected and cleaned data to extract landing outcomes as labels for machine learning.
- **Visualization:**  
  Used SQL queries, static and interactive charts, Folium maps, and a Plotly Dash dashboard.
- **Prediction:**  
  Applied and compared Logistic Regression, SVM, Decision Tree, and K-Nearest Neighbors (KNN) models.

---

## Introduction

The commercial space race is highly competitive.  
**Objective:** Predict the success of Falcon 9 first stage landings to estimate costs and optimize operations.

**Key Questions:**
- What patterns can be found in historical Falcon 9 launch data?
- Which ML model gives the highest prediction accuracy for landings?
- What insights can be drawn from launch sites, payloads, orbits, and booster versions?

---

## Methodology

1. **Data Collection**  
   - Downloaded launch data via SpaceX API, Wikipedia tables, and CSV files.
2. **Data Cleaning & Wrangling**  
   - Reformatted mission outcomes into binary labels (success/failure).
   - Processed categorical variables and handled missing values.
3. **Exploratory Data Analysis (EDA)**  
   - Visualized data trends by launch site, payload, orbit, and date.
   - Used both SQL and Python for querying and plotting.
4. **Geospatial Analysis**  
   - Used Folium maps to analyze launch site proximities and outcomes.
5. **Interactive Dashboard**  
   - Built with Plotly Dash for interactive data exploration and visualization.
6. **Predictive Modeling**  
   - Split data into train/test sets.
   - Trained and tuned Logistic Regression, SVM, Decision Tree, and KNN.
   - Compared models using test accuracy and confusion matrices.

---

## Results

- **EDA Insights:**  
  - Success rates vary significantly by launch site and orbit type.
  - Later flights show a higher landing success rate in the saved course dataset.
  - Payload and booster categories show differing outcomes in the exploratory charts.
- **Dashboard Insights:**  
  - Interactive site and payload filtering visualized patterns in success/failure rates.
  - KSC LC-39A had the most successful landings; CCAFS SLC-40 had the highest success rate.
- **Model Performance:**  
  - All four models reported **83.3% test accuracy** on a small 18-record holdout set.
  - The saved Decision Tree confusion matrix contains 3 false positives and no false negatives. This small sample is insufficient for a production claim.

---

## Conclusion

- SpaceX Falcon 9 landing success rates have significantly improved over time.
- All evaluated machine learning models provided similar predictive power on this dataset.
- Visual analysis and models support exploratory discussion, but they do not constitute a validated launch-risk system.
- **Methodological limitation:** Feature scaling was fit before the train/test split in the saved modeling notebook. Re-evaluation with preprocessing inside cross-validation is recommended to avoid leakage.

---

## Appendix & References

**Key Notebooks & Files:**
- `Module1/`: Data collection, scraping, wrangling notebooks and CSVs
- `Module2/`: SQL EDA notebook
- `Module3/`: Visualization, dashboard code, screenshots
- `Module4/`: ML modeling and evaluation notebooks
- [Module5/](Module5/): final presentation guide, delivery files and evidence checklist

**Data Sources:**
- [SpaceX Public API](https://api.spacexdata.com/)
- [Wikipedia: List of Falcon 9 and Falcon Heavy launches](https://en.wikipedia.org/wiki/List_of_Falcon_9_and_Falcon_Heavy_launches)
- IBM Course-provided datasets (CSV)
  
**Author:**  
Kardelen Geçkin  
[LinkedIn](https://www.linkedin.com/in/krgckn/)

---

