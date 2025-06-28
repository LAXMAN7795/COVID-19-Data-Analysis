# 🌍 COVID-19 Data Analysis

## 🧠 Problem Statement
Understanding COVID-19 trends is crucial for making informed public health decisions. This project analyzes global COVID-19 data to visualize trends and compare country-level statistics.

---

## 🎯 Objective
- Analyze global COVID-19 data (Confirmed, Recovered, Deaths).
- Visualize cumulative trends.
- Compare top-affected countries.
- Understand correlations between metrics.

---

## 📁 Dataset
- **Source**: `country_wise_latest.csv` (assumed pre-processed snapshot of global data).
- **Key Columns**:
  - `Country/Region`
  - `Confirmed`
  - `Recovered`
  - `Deaths`

---

## 🔧 Data Preprocessing
- Dropped irrelevant columns:
  - Active cases, ratios, last week metrics, WHO region.
- Checked for missing values (no significant nulls found).
- Cleaned data was used for all visualizations.

---

## 📊 Visualizations

### 📈 1. Line Plots
- For the top 5 countries by confirmed cases.
- Shows `Confirmed`, `Recovered`, `Deaths` as separate points for each country.
- Saved figures as: `CountryName_covid_summary.png`.
![image](https://github.com/LAXMAN7795/COVID-19-Data-Analysis/blob/89b2bcb4685bd99ba286383885a6f5f6ed8d5fba/output/US_covid_summary.png)
![image](https://github.com/LAXMAN7795/COVID-19-Data-Analysis/blob/37fd260f300a5a4d6704f7c8702020111918087f/output/Brazil_covid_summary.png)
![image](https://github.com/LAXMAN7795/COVID-19-Data-Analysis/blob/574160f0824d411d16bbed29fdad71ba2b141f1f/output/India_covid_summary.png)
![image](https://github.com/LAXMAN7795/COVID-19-Data-Analysis/blob/a7fe699d84543e982e183e5f4607c896a4bebddc/output/Russia_covid_summary.png)
![image](https://github.com/LAXMAN7795/COVID-19-Data-Analysis/blob/7ca24677dbf0bcdd03445d5c0eb7f133b9df41d3/output/South%20Africa_covid_summary.png)

### 🟧 2. Area Chart
- Stacked area chart for top 3 countries by confirmed cases.
- Visual comparison of the spread and recovery over time.
- Saved as: `covid_area_chart.png`.

![image](https://github.com/LAXMAN7795/COVID-19-Data-Analysis/blob/6badd9b44e90c3bf02f35b0b5eb3e09e5a3810d8/output/covid_area_chart.png)

### 🔥 3. Heatmap
- Correlation heatmap between `Confirmed`, `Recovered`, and `Deaths`.
- Highlights relationships among key metrics.

---

## 📌 Key Insights
- Countries with high confirmed cases often also show high recovery counts.
- Strong correlation between confirmed and recovered cases.
- Mortality rates vary significantly among countries.

---

## ✅ How to Run
1. Ensure `country_wise_latest.csv` is in the same directory as the notebook.
2. Run the Jupyter Notebook (`.ipynb`) step by step.
3. Visual outputs will be displayed and saved as PNG files.

---

## 📚 Requirements
- Python
- pandas
- numpy
- matplotlib
- seaborn
