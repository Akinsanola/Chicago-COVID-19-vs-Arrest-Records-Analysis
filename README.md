# 🦠 Chicago Crime & COVID-19: An Exploratory Data Analysis (2020-2022)

---

## Project Overview

This project is an **Exploratory Data Analysis (EDA)** investigating the relationship between **COVID-19 pandemic metrics** and **reported crime rates** in Chicago from 2020 to 2022. It was completed as a core project for an introductory Data Science course.

The primary goal was to perform data acquisition, cleaning, **integration (ETL)**, and descriptive visualization of two large, disparate public datasets. The analysis focuses on uncovering initial trends, community-level disparities, and patterns in how public health crises and social dynamics interact in a major urban center.

---

## 🛠️ Technical Stack & Scope

* **Project Scope:** **Exploratory Data Analysis (EDA)**, Data Cleaning, Data Integration, and Descriptive Visualization.
* **Programming Language:** **R** (Analysis performed within a Quarto Document).
* **Data Processing:** **ETL** involving filtering, merging by community area and week numbers, and computing weekly crime counts.
* **Data Sources:** All data was sourced from the Chicago Data Portal:
    * COVID-19 Cases, Tests, and Deaths by ZIP Code Historical: [Link](https://data.cityofchicago.org/Health-Human-Services/COVID-19-Cases-Tests-and-Deaths-by-ZIP-Code-Histor/yhhz-zm2v/about_data)
    * Arrests: [Link](https://data.cityofchicago.org/Public-Safety/Arrests/dpt3-jri9/about_data)
    * COVID-19 Daily Cases, Deaths, and Hospitalizations: [Link](https://data.cityofchicago.org/Health-Human-Services/COVID-19-Daily-Cases-Deaths-and-Hospitalizations-H/naz8-j4nc/about_data)

---

## 📊 Core Exploratory Findings

The analysis successfully identified significant spatial and temporal differences in both crime and pandemic severity.

* **Community Disparities (Crime):**
    * **Highest Crime (2020-2022):** Near North Side, Austin, and Near West Side were observed to have the highest total crime counts.
    * **Pre-Pandemic Shift:** Total crime counts increased significantly during the pandemic in several urban centers (e.g., Near North Side and Austin) compared to the 2019 baseline.
* **Community Disparities (COVID-19 Severity):**
    * **Highest Positivity Rate:** Montclare, Riverdale, and Chicago Lawn.
    * **Highest Average Deaths:** Gage Park, Chicago Lawn, and West Lawn.
* **Testing Correlation:** A **strong positive correlation ($\text{0.903}$)** was found between weekly testing rates and reported case counts across ZIP codes, suggesting higher testing efforts lead to higher reported cases.

---

## 🗺️ Future Work & Replication Roadmap

This project provides a robust, cleaned dataset and initial findings that lay the foundation for more advanced data science work.

| Phase | Objective | Recommended Techniques |
| :--- | :--- | :--- |
| **Phase 1: Causality & Regression** | Quantify the statistical relationship between pandemic metrics and crime rates. | **Statistical Regression:** Use crime rate as the dependent variable to test predictors like positivity rate, testing rates, and population density. |
| **Phase 2: Predictive Modeling** | Predict short-term crime trends or future case rates using time-series data. | **Time Series Models:** ARIMA, SARIMA, or Prophet for forecasting crime or COVID-19 metrics. |
| **Phase 3: External Data Integration** | Provide deeper socio-economic context for the crime disparities observed across neighborhoods. | **External Data Integration:** Incorporate external variables (e.g., unemployment rates, median income, public transportation usage) using data from the Census Bureau or similar sources. |

---

## 📁 Repository Structure

* `Chicago_Crime.pdf`: The full project report detailing the methodology, analysis, and findings. **(Highly Recommended to view first!)**
* `Ololade_Akinsanola_Project_Phase3qmd.qmd`: **R/Quarto source code file** containing all data cleaning, transformation, analysis, and visualization code.
