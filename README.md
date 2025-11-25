## Heart & Kidney Disease Statistical Analysis

This repository contains an R-based statistical analysis exploring the relationship between heart disease and kidney disease. The goal is to test whether the proportion of people with kidney disease is higher among those with heart disease compared to those without.

## Dataset

The analysis uses the `heart_2020_cleaned.csv` dataset, which contains survey data with indicators for heart disease, kidney disease, and other health-related variables. The data includes hundreds of thousands of observations with features such as BMI, physical and mental health indicators, and chronic conditions.

The dataset is taken from the Kaggle “Personal Key Indicators of Heart Disease” dataset, which is derived from the CDC’s 2020 Behavioral Risk Factor Surveillance System (BRFSS) survey.

## Methods

All analysis is implemented in **RMarkdown** (`main.Rmd`) and rendered to `main.html`. The workflow includes:

- Cleaning and selecting relevant variables for heart disease and kidney disease  
- Exploratory summaries of the two groups (with and without heart disease)  
- Constructing a **two-proportion hypothesis test** to compare:
  - proportion of kidney disease in the heart-disease group  
  - vs. proportion of kidney disease in the non–heart-disease group  
- Computing the test statistic and p-value  
- Building a confidence interval for the difference in proportions  
- Visualizing the estimated difference and interval using `ggplot2`

Key R packages used include:

- `readr` for loading the dataset  
- `dplyr` for data wrangling  
- `ggplot2` for visualization  
