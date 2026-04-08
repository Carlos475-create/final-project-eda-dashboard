# COVID-19 and Vaccination Analysis

## 📌 Project Overview

This project analyzes the relationship between COVID-19 cases, deaths, and vaccination progress across countries. The goal is to understand global trends, compare countries, and evaluate whether vaccination levels are directly associated with pandemic outcomes.

---

## 📊 Data Sources

Two datasets from different sources were used:

- COVID-19 dataset (cases and deaths)
- Vaccination dataset (vaccination metrics)

Both datasets were merged using:
- `Country_code`
- `Date`

---

## 🧹 Data Cleaning & Transformation

The following steps were performed:

- Merged datasets using a left join on `Country_code` and `Date`
- Converted date columns to datetime format
- Sorted data by country and date
- Removed duplicate records
- Handled missing values:
  - Vaccination data was left as NaN where appropriate, assuming structurally missing data (MNAR)
- Created time-based features (e.g., monthly aggregation where necessary)

---

## 📈 Exploratory Data Analysis (EDA)

The analysis focused on:

### 🌍 Global Trends
- Evolution of new cases and deaths over time
- Identification of pandemic waves

### 🌎 Country Comparison
- Top 10 countries by cumulative cases
- Top 10 countries by cumulative deaths

### 💉 Vaccination Analysis
- Top countries by total vaccinations administered
- Comparison between vaccination levels and pandemic outcomes

### 🔗 Correlation Analysis
- Correlation between:
  - Cases
  - Deaths
  - Vaccination variables

---

## 🔍 Key Insights

- There is **no strong linear relationship** between vaccination levels and new COVID-19 cases or deaths.
- A **moderate correlation** exists between new cases and deaths, which aligns with expected pandemic behavior.
- Vaccination variables are **highly correlated among themselves**, indicating redundancy (multicollinearity).
- Countries with large populations dominate rankings in absolute values.
- An interesting case is **China**, which:
  - Has high cumulative cases
  - Leads in vaccine administration
  - Does not appear in the top 10 for deaths  
  This highlights the importance of considering population size, policies, and reporting differences.

---

## ⚠️ Limitations

- Analysis is based on **absolute values**, not normalized metrics
- Differences in reporting standards between countries may affect results
- Time-lag effects between vaccination and outcomes are not captured
- Cumulative metrics may obscure short-term dynamics

---

## 🛠️ Tools & Technologies

- Python
  - Pandas
  - Matplotlib
  - Seaborn
- Visual Studio Code
- Excel (for dashboard)

---

## 📊 Dashboard

The dashboard includes:

- Global trends of cases and deaths
- Top countries by cases and deaths
- Vaccination distribution
- Relationship between vaccination and cases

---

## 📌 Conclusion

This analysis shows that the impact of vaccination on COVID-19 outcomes is complex and cannot be explained by simple correlations. Multiple factors such as population size, policy measures, and timing play a critical role in shaping pandemic dynamics.

---

## 🚀 Next Steps

- Normalize data by population (per 100k)
- Include time-lag analysis
- Incorporate additional variables (mobility, policies)




# 🧠 Analysis of COVID-19 and Vaccination Data

This project explores the relationship between COVID-19 cases, deaths, and vaccination progress across countries using a merged dataset from two independent sources.

## 📈 Global Trends

The analysis of global trends shows clear waves of infection over time, reflecting the different phases of the pandemic. Peaks in new cases are followed by increases in deaths, although not perfectly aligned, indicating delays and variability in outcomes.

## 🌍 Country-Level Analysis

The comparison of countries reveals that a small number of countries account for a large proportion of total cases and deaths. Countries such as the United States, India, and Brazil consistently appear among the most affected.

However, this distribution is strongly influenced by population size, meaning that absolute values alone may not provide a complete picture.

## 💉 Vaccination Analysis

Vaccination data shows that countries like China, India, and the United States lead in total vaccine administration. However, vaccination metrics are highly correlated with each other, indicating that they measure similar aspects of vaccine rollout.

## 🔗 Correlation Findings

The correlation analysis reveals:

Weak correlation between vaccination variables and both new cases and deaths
Moderate positive correlation between new cases and deaths
Strong correlation among vaccination variables (multicollinearity)

These findings suggest that the effect of vaccination is not directly observable through simple linear relationships.

## 📌 Key Insight: The Case of China

A notable finding is that China ranks among the countries with the highest cumulative cases and has the highest number of vaccine doses administered, yet it does not appear among the top countries in cumulative deaths.

This may be explained by:

Strict public health measures
High vaccination coverage
Differences in reporting practices
Timing of pandemic waves

This observation highlights the importance of considering contextual and structural factors when interpreting data.

## ⚠️ Limitations of the Analysis
Use of cumulative and absolute values instead of normalized metrics
Lack of time-lag consideration between vaccination and outcomes
Potential inconsistencies in international reporting standards
## 📊 Final Conclusion

The analysis demonstrates that COVID-19 outcomes are influenced by a complex interaction of factors. While vaccination plays a crucial role, its impact cannot be fully captured through simple correlation analysis. A deeper, more nuanced approach is required to understand pandemic dynamics.
