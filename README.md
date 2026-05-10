# Private School Access and Education Opportunity in Texas

## Overview

I started this project to better understand how educational opportunity varies across Texas. As a private-school student, I wanted to look beyond my own experience and use public data to study how private-school access differs across counties.

This project analyzes the relationship between private-school access, income, poverty, population, and adult education level in Texas counties.

## Research Question

How does private-school access vary across Texas counties, and how is it related to income, poverty, and adult education level?

## Data Sources

- NCES Private School Universe Survey
- U.S. Census ACS 5-Year county-level data
- County-level dataset created with Python and pandas

## Methods

I cleaned and combined private-school and Census county-level data, then calculated private-school access as:

> private schools per 100,000 people

I used:

- data cleaning
- county-level aggregation
- correlation analysis
- data visualization
- linear regression

## Key Findings

- Across all Texas counties, median income had almost no correlation with private-school access.
- Among counties with populations above 50,000, median income had a weak positive relationship with private-school access.
- Poverty rate had a weak negative relationship with private-school access.
- Adult education level had the strongest relationship with private-school access.
- In the regression model, bachelor's degree attainment was the only statistically significant predictor among the variables tested.

## Main Result

Private-school access in larger Texas counties appears to be more strongly associated with adult education level than with median income or poverty rate alone.

## Visualizations

### Adult Education Level and Private School Access
![Adult Education Level and Private School Access](charts/education_vs_private_school_access.png)

### Private School Access by Income Group
![Private School Access by Income Group](charts/private_school_access_by_income_group.png)

### Poverty Rate and Private School Access
![Poverty Rate and Private School Access](charts/poverty_vs_private_school_access.png)

### Median Income and Private School Access
![Median Income and Private School Access](charts/income_vs_private_school_access_population_50000_plus.png)

## Tools Used

- Python
- pandas
- matplotlib
- statsmodels
- Google Colab
- GitHub

## Limitations

This project shows association, not causation. County-level analysis can hide important differences within counties, and private-school access may also depend on factors such as religion, urbanization, local history, transportation, and family preferences.
