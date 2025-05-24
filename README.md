# Florida Crime Data Regression Analysis

**Author:** Cassidy Halpin  
**Course:** MIS500-1 – Foundations of Data Analytics  
**Date:** October 6, 2024  

## Project Overview

This project analyzes crime rates across counties in Florida using linear and stepwise regression techniques. The primary goal is to determine the influence of **Income**, **High School Graduation Rate (HS)**, and **Urbanization (Urban)** on the **Crime** variable using statistical modeling in SAS Enterprise Miner.

The analysis begins with a standard linear regression model and is refined using a stepwise regression approach to select the most statistically significant predictors.

## Key Objectives

- Evaluate the effect of socio-economic variables on county-level crime rates  
- Use linear regression to estimate contributions of Income, HS, and Urban  
- Apply stepwise selection to identify the best-fitting predictive model  
- Interpret statistical outputs including p-values, R-squared, and ANOVA  
- Assess residuals and diagnostic plots for model performance  

## Tools & Methods

- **Software:** SAS Enterprise Miner  
- **Dataset:** Crime in Florida.csv  
- **Methods Used:**
  - Multiple Linear Regression  
  - Stepwise Regression  
  - Residual Diagnostics  
  - Visualization: Observed vs. Predicted Plots  

## Model Results Summary

### Linear Regression (Initial Model)
- **F-value:** 18.83 (p < 0.0001) → Statistically significant model  
- **R²:** 0.4728 → ~47.28% of crime variance explained  
- **Significant Predictor:**  
  - **Urban** (p < 0.0001)  
- **Non-significant Predictors:**  
  - **Income** (p = 0.6852)  
  - **HS Graduation Rate** (p = 0.4025)  
- **Diagnostics:** Plots revealed minor variance patterns, indicating room for model improvement.

### Stepwise Regression (Refined Model)
- **Selected Predictor:** Urban (via Schwarz Bayesian Criterion)
- **F-value:** 55.11 (p < 0.0001)  
- **R²:** 0.4588, **Adjusted R²:** 0.4505  
- **Urban Coefficient:** 0.562  
  - A 1-unit increase in Urban leads to a predicted 0.562 unit increase in Crime  
- **Total Sum of Squares:** 52,462  
- **Diagnostics:** Minor heteroscedasticity observed—future improvement possible with transformation or additional predictors.

## Key Insights

- Urbanization is a **highly significant** predictor of crime rates in Florida counties.  
- Neither Income nor HS Graduation Rate showed statistically significant impacts on crime in this dataset.  
- The refined model explains ~46% of crime variance, leaving room for future enhancement.  
- Diagnostic plots suggest decent fit but hint at potential heteroscedasticity issues.

## Conclusion

This project demonstrates how regression modeling can extract actionable insights from public crime data. The use of stepwise regression effectively narrowed down the most impactful variable (Urbanization), allowing for a more focused and interpretable model. The experience reinforced the importance of proper variable selection, diagnostic evaluation, and the limitations of purely statistical approaches without incorporating broader socio-contextual variables.

---

> **Figures & Code:**  
> - Figures 1–12 document the modeling process, regression outputs, diagnostics, and code.  
> - Available in the Fall Portfolio document

