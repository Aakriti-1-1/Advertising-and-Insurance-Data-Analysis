# Advertising-and-Insurance-Data-Analysis
Statistical analysis of advertising effectiveness and health insurance cost drivers using Python, EDA, Correlation and Multiple Linear Regression.

**Business Analytics | Exploratory Data Analysis | Statistical Modelling | Multiple Linear Regression**

A Python-based analytics project exploring two business problems: advertising effectiveness and health insurance cost drivers. Uses statistical analysis and multiple linear regression to identify significant predictors, evaluate model performance, and derive actionable business insights.

## Project Objectives

- Identify advertising channels associated with higher sales.
- Quantify the relationship between advertising expenditure and sales performance.
- Investigate demographic and lifestyle factors influencing health insurance charges.
- Build and evaluate multiple linear regression models.
- Translate statistical findings into business recommendations.

## Tech Stack

`Python` `Pandas` `NumPy` `SciPy` `Statsmodels` `Matplotlib` `Seaborn` `Jupyter Notebook`

## 1. Advertising Sales Analysis

**Dataset:** 200 observations | 4 variables

Analysed the relationship between TV, Radio and Newspaper advertising expenditure and sales using correlation analysis and OLS multiple linear regression.

### Key Results

**Correlation with Sales**

| Channel | Correlation |
|---|---:|
| TV | 0.90 |
| Radio | 0.35 |
| Newspaper | 0.16 |

**Regression Model Performance**

| Metric | Result |
|---|---:|
| R-squared | 90.3% |
| Adjusted R-squared | 90.1% |
| F-statistic | 605.4 |

**Regression Coefficients**

| Variable | Coefficient | P-value |
|---|---:|---:|
| TV | 0.0544 | <0.001 |
| Radio | 0.1070 | <0.001 |
| Newspaper | 0.0003 | 0.954 |

### Business Insights

- **TV:** Strongest relationship with sales and a statistically significant predictor.
- **Radio:** Demonstrates a significant positive contribution to sales.
- **Newspaper:** No statistically significant independent contribution in the fitted model.
- **Strategic Implication:** Prioritise evaluating TV and Radio investments while reassessing Newspaper advertising effectiveness.

## 2. Health Insurance Cost Analysis

**Dataset:** 1,338 observations | 7 variables

Investigated the influence of Age, BMI and Smoking Status on individual medical insurance charges using multiple linear regression and categorical variable encoding.

### Model Comparison

| Model | Predictors | R-squared |
|---|---|---:|
| Model 1 | Age + BMI | 11.7% |
| Model 2 | Age + BMI + Smoking Status | 74.7% |

### Final Regression Results

| Variable | Coefficient (approx.) | P-value |
|---|---:|---:|
| Age | 259.55 | <0.001 |
| BMI | 322.62 | <0.001 |
| Smoker (Yes) | 23,820 | <0.001 |

**Final Model Performance**

- R-squared: 74.7%
- Adjusted R-squared: 74.7%
- F-statistic: 1,316
- Observations: 1,338

### Business Insights

- **Smoking Status:** Strongest predictor in the model. Smokers have estimated insurance charges approximately 23,820 monetary units higher than non-smokers, holding other predictors constant.
- **Age:** Each additional year is associated with an estimated increase of 259.55 monetary units in charges.
- **BMI:** Each additional BMI unit is associated with an estimated increase of 322.62 monetary units in charges.
- **Strategic Implication:** Incorporating lifestyle and demographic indicators can substantially improve insurance cost modelling and customer risk segmentation.

## Analytical Techniques

- Exploratory Data Analysis (EDA)
- Descriptive Statistics: Mean, Median, Standard Deviation, Skewness and Kurtosis
- Correlation Matrix
- Jarque-Bera Normality Test
- Augmented Dickey-Fuller (ADF) Test
- Phillips-Perron Test
- Elliott-Rothenberg-Stock (ERS / DF-GLS) Test
- Categorical Encoding and Dummy Variable Creation
- Ordinary Least Squares (OLS) Regression
- Model Evaluation: R-squared, Adjusted R-squared, F-statistic and P-values
- Regression Diagnostics: Residual Distribution, Box Plot and Q-Q Plot

## Key Takeaways

1. TV and Radio advertising are statistically significant predictors of sales, with the advertising model explaining 90.3% of sales variation.
2. Smoking Status substantially improves insurance cost model performance, increasing explanatory power from 11.7% to 74.7%.
3. Regression modelling provides measurable evidence to support marketing investment evaluation and insurance risk assessment.

## Repository Structure

```text
Insurance-Advertising-Analytics/
│
├── Insurance&Advertising_9236.ipynb
├── advertising.csv
├── insurance[1].csv
└── README.md
```

## Future Scope

- Test model performance on unseen data.
- Explore interaction effects and nonlinear relationships.
- Incorporate additional predictors into insurance modelling.
- Compare OLS with regularised and tree-based regression models.
- Evaluate predictive accuracy using RMSE and MAE.
- Apply robust regression diagnostics and validation.

## Conclusion

This project demonstrates the application of statistical modelling to practical business problems. By identifying significant sales drivers and insurance cost determinants, it showcases the use of Python-based analytics to derive interpretable insights and support evidence-based managerial decision-making.

---

**Project Domain:** Marketing Analytics | Insurance Analytics | Business Intelligence
