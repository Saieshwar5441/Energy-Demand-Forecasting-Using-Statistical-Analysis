# Energy-Demand-Forecasting-Using-Statistical-Analysis

This project involves a comprehensive statistical analysis of energy consumption across Eastern (PJME) and Western (PJMW) regions of the United States. Using time series data provided by PJM Interconnection, the project leverages visualization, correlation analysis, hypothesis testing, and predictive modeling techniques to uncover trends, seasonal patterns, and inter-regional relationships.

## Why We Did This Project

We wanted to **analyze electricity consumption trends across the year** and identify **which periods experience peak demand**. By using statistical techniques, we aimed to uncover:

- **When** electricity consumption is at its highest (e.g., by season, month, weekday)
- **What factors** (e.g., time of year, day of the week, regional differences) significantly influence energy demand
- Whether **seasonal variation** and **regional correlation** can help **predict energy usage** and guide infrastructure planning

This analysis helps energy providers, urban planners, and policy makers make **data-informed decisions** for **demand management**, **load balancing**, and **resource allocation**.

---

## Course Information

- **Course:** MA541 – Statistical Methods  
- **Semester:** Fall 2024  
- **Team Members:**  
  - Sai Eshwar Gaddipati  
  - Vedanth Sirimalla  
  - Shachee Bhatt  
  - Rajashekhar Manyam  

---

## Dataset Description

- **Source:** PJM Interconnection (via public hourly datasets)  
- **Period Covered:** January 2002 – August 2018  
- **Variables:**  
  - `PJME_MW` – Power consumption in Eastern region  
  - `PJMW_MW` – Power consumption in Western region  
  - Time-based features: hour, weekday, month, year, season  

---

## Key Statistical Analyses

### Exploratory Analysis
- Descriptive statistics (mean, std, percentiles)
- Time series trends and seasonal patterns
- Histograms, scatter plots, and correlation heatmaps

### Feature Engineering
- Derived season, hour, weekday, month, quarter, year, etc.
- Combined datasets for aligned temporal analysis

### Correlation & Hypothesis Testing
- **Pearson correlation:** PJME vs PJMW → r = 0.876, p = 0.0
- **ANOVA:** Seasonal electricity consumption is statistically different  
- **Kruskal-Wallis test:** Confirms variation in medians across seasons

### Predictive Modeling
- **Linear Regression (PJMW ~ PJME):**  
  - R² = 0.768 → 76.8% variance explained  
  - MSE = 0.0027  
- **ANOVA Test:**  
  - F-statistic = 2,349,712.44, p = 0.0 → highly significant

---

## Visualizations

- Time series plots for PJME and PJMW  
- Box plots across seasons, months, and quarters  
- Histograms with seasonal hue  
- Heatmaps for correlation strength  
- Scatter plots for inter-regional relationships  

## 🧾 Summary Insights

| Aspect               | PJME (East)            | PJMW (West)              |
|----------------------|------------------------|--------------------------|
| Mean Consumption     | 32,080.5 MW            | 5,602.4 MW               |
| Std. Deviation       | 6,464.0 MW             | 979.1 MW                 |
| Seasonal Peak        | Winter & Summer        | Winter & Summer          |
| Correlation          | r = 0.876              | r = 0.876                |
| R² (Linear Model)    | —                      | 0.768                    |


