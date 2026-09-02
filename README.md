#  Housing Price Modeling: A Statistical Approach

![Language](https://img.shields.io/badge/Language-R-blue)
![Course](https://img.shields.io/badge/Course-Applied_Linear_Models-brightgreen)
![Status](https://img.shields.io/badge/Status-Completed-success)

##  Overview
This repository contains the final project for the **Applied Linear Models** course. The study presents a comprehensive statistical analysis and predictive modeling of 2023 New York housing prices. By applying advanced multiple linear regression techniques, the analysis identifies the most significant property attributes influencing market values and provides a robust framework for price estimation.

##  Academic Context
* **Author:** Giorgia Cappellato
* **Course:** Applied Linear Models
* **Academic Year:** 2024/2025
* **Institution:** Università Cattolica del Sacro Cuore

##  Dataset
The analysis is based on a New York housing dataset (sourced from Kaggle) containing **545 observations and 13 variables**. 
The dependent variable is the property `price`, while independent variables include structural characteristics (e.g., `area`, `bedrooms`, `bathrooms`, `stories`) and categorical amenities (e.g., `airconditioning`, `parking`, `guestroom`).

##  Statistical Methodology
The project follows a rigorous statistical workflow to ensure the reliability of the predictive model:

1. **Data Transformation:** Applied a log-transformation to the response variable (`Price`) to normalize right-skewness, stabilize variance (addressing heteroscedasticity), and ensure compliance with linear model assumptions.
2. **Variable Selection:** Performed an exhaustive subset selection algorithm. The optimal model complexity was evaluated using multiple criteria: **AIC, BIC, Mallows' Cp, Adjusted R-squared**, and **k-fold Cross-Validation**.
3. **Multicollinearity Check:** Computed the Generalized Variance Inflation Factor (GVIF).
4. **Model Diagnostics:** 
   * **Linearity & Homoscedasticity:** Evaluated through Residuals vs. Fitted plots.
   * **Normality:** Confirmed via Q-Q plots, histograms, and formally validated by the **Shapiro-Wilk test**.
   * **Unusual Observations:** Analyzed Studentized residuals, Leverage points, and Cook's Distance to ensure no single observation had an undue influence on the estimates.

##  Key Results
* **Model Performance:** The final linear regression model explains **67.82% of the variance** in housing prices.
* **Significant Predictors:** The most impactful variables on price increases include `area`, `bathrooms`, `basement`, and `airconditioning`.
* **Simulation & Calibration:** Model simulations with added random noise closely mirrored observed data, confirming the model's reliability for real-world predictions.

##  Technologies & Tools
* **Language:** R
* **Methods:** Multiple Linear Regression, ANOVA, Cross-Validation, Statistical Diagnostics.
* **Outputs:** RMarkdown for reproducible research (`.Rmd`).

## 🚀 How to Run the Project

1. Clone the repository:
   ```bash
   git clone [https://github.com/giorgiacappellato/housing-price-modeling.git](https://github.com/giorgiacappellato/housing-price-modeling.git)
