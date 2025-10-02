# EPL Outcome Analytics

Predicting English Premier League (EPL) match outcomes and analyzing key performance metrics using classical statistical models and feature engineering.

---

## 📂 Project Overview

This project focuses on understanding the factors influencing EPL match outcomes. Using historical match data, we explore correlations, build predictive models, and derive actionable insights.

**Key objectives:**

* Analyze match statistics and team performance trends.
* Predict home goals and match results using statistical models.
* Explore momentum and contextual factors affecting match outcomes.
* Highlight interpretable and explainable results.

---

## 🗃️ Dataset

* **Source:** English Premier League match results (`results.csv`).
* **Timeframe:** 2015–16 season onwards.
* **Selected columns:** `Season`, `DateTime`, `HomeTeam`, `AwayTeam`, `FTHG`, `FTAG`, `FTR`, `HST`, `AST`, `HC`, `AC`, `HF`, `AF`, `Weekday`.
* **Focus:** Numeric and categorical variables influencing match outcomes.

---

## 🔍 Exploratory Data Analysis (EDA)

* **Correlation analysis:** Home shots on target (`HST`) strongly influence home goals (`FTHG`).
* **Categorical analysis:** Referees show some bias; weekday has no significant effect.
* **ANOVA:** Home shots on target vary significantly across match results.
* **Seasonal trends:** Slight upward trend in goals over recent seasons.

---

## 🧮 Modeling

1. **Poisson Regression** – Predicting home goals based on match statistics.
2. **Multinomial Logistic Regression** – Predicting match outcomes (H/D/A).
3. **Binomial GLM** – Home win vs not, incorporating a novel metric: **HomeMomentum**.
4. **Exponential Smoothing** – Forecasting average home goals for future seasons.

**Highlights:**

* Statistically significant predictors identified.
* Models validated using AIC/BIC and residual diagnostics.
* Insights are interpretable and explainable.

---

## 💡 Key Insights

* Teams with **higher HomeMomentum** are more likely to win home games.
* Home shots on target (`HST`) are the strongest driver of home goals.
* Certain referees influence outcomes statistically.
* Corners and fouls impact possession, momentum, and scoring.
* Underdogs perform better when away team shots on target are low.

---

## 📊 Visualizations

* Correlation heatmaps for numeric predictors vs goals.
* Chi-square tables for categorical predictors vs match outcomes.
* Boxplots and histograms: HomeMomentum vs match result.
* Scatterplots: HomeMomentum vs home goals.
* Seasonal trends: average goals per season.
* Residual histograms for Poisson & GLM model validation.

---

## 🔧 Requirements

* Python >= 3.8
* Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `statsmodels`, `scikit-learn`
* Jupyter Notebook or similar environment for running analyses

---

## 📝 Conclusion

This project demonstrates a **classical statistical approach** to sports analytics. Insights are fully interpretable, models are explainable, and novel metrics like **HomeMomentum** enhance prediction quality.

---


