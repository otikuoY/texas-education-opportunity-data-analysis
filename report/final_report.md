# Private School Access and Education Opportunity in Texas

## Abstract

This project analyzes how private-school access varies across Texas counties and how it relates to income, poverty, and adult education level. I combined private-school data, Census county-level data, and basic statistical analysis to compare private-school access across Texas counties. The main measure of access was the number of private schools per 100,000 people.

The analysis found that median household income had almost no relationship with private-school access across all Texas counties. Among counties with populations above 50,000, income showed a weak positive relationship, while poverty rate showed a weak negative relationship. The strongest relationship was with adult education level: counties with higher percentages of adults holding bachelor's degrees or higher tended to have greater private-school access.

## Introduction

Educational opportunity is not distributed evenly across communities. As a private-school student in Texas, I wanted to look beyond my own school experience and use public data to better understand how private-school access varies across the state.

This project focuses on Texas counties because county-level data makes it possible to compare private-school access with broader social and economic indicators such as income, poverty, population, and adult education level.

## Research Question

How does private-school access vary across Texas counties, and how is it related to income, poverty, and adult education level?

## Data Sources

This project used three main types of data:

- NCES Private School Universe Survey data for private-school information
- U.S. Census ACS county-level data for population, median income, poverty, and adult education level
- County-level aggregation created in Python using pandas

The final dataset measured private-school access using private schools per 100,000 people.

## Methods

First, I cleaned the private-school dataset and filtered it to only include Texas schools. I selected key columns such as school name, state, county, city, enrollment, teacher count, and student-teacher ratio.

Next, I grouped the private-school data by county to calculate:

- total number of private schools
- total private-school enrollment
- total private-school teacher count
- private schools per 100,000 people
- private enrollment per 100,000 people

Then I cleaned the Census county-level data and merged it with the private-school county summary. Counties with no private schools were included and assigned a private-school count of zero.

I then calculated correlations between private-school access and several county-level indicators. I also focused on counties with populations above 50,000 to reduce distortion from very small counties, where per-100,000 measures can become unusually large.

Finally, I ran a linear regression model using median income, poverty rate, adult education level, and population to see which variables were most strongly associated with private-school access.

## Results

### Correlation Results

- Median income and private-school access across all Texas counties: 0.039
- Median income and private-school access among counties with population 50,000+: 0.284
- Poverty rate and private-school access among counties with population 50,000+: -0.151
- Bachelor's degree or higher percentage and private-school access among counties with population 50,000+: 0.446

Across all Texas counties, median household income had almost no relationship with private-school access. Among counties with populations above 50,000, income showed a weak positive relationship.

Poverty rate showed a weak negative relationship, meaning counties with higher poverty rates tended to have slightly fewer private schools per 100,000 people.

The strongest relationship was with adult education level. Counties with higher percentages of adults holding bachelor's degrees or higher tended to have greater private-school access.

### Regression Results

The regression model had an R-squared value of 0.212, meaning it explained about 21.2% of the variation in private-school access among counties with populations above 50,000.

In the regression model, bachelor's degree attainment was the only statistically significant predictor among the variables tested. Median income, poverty rate, and population were not statistically significant predictors.

This suggests that private-school access in larger Texas counties may be more strongly associated with adult education level than with income or poverty alone.

## Key Finding

The main finding of this project is that private-school access is not explained well by income alone. Adult education level appears to have a stronger relationship with private-school access than median household income or poverty rate.

This does not mean that adult education level causes private-school access. It only means that, in this dataset, counties with higher adult education levels tended to have more private schools per 100,000 people.

## Limitations

This project has several limitations.

First, the analysis is correlational, not causal. The results show relationships between variables, but they do not prove that one variable causes another.

Second, the analysis is county-level. Counties can contain very different communities, so county averages may hide important differences between neighborhoods, cities, and school zones.

Third, private-school access may depend on factors not included in this model, such as religion, urbanization, local history, school choice culture, transportation, and family preferences.

Fourth, the regression model explained only part of the variation in private-school access. This means other factors likely play an important role.

## Conclusion

This project started with a simple question: how does private-school access vary across Texas counties, and how is it related to local economic and educational conditions?

The results showed that income alone does not explain private-school access very well. Among larger Texas counties, adult education level had the strongest relationship with private-school access. Counties with higher percentages of adults holding bachelor's degrees or higher tended to have more private schools per 100,000 people.

Overall, this project showed me that data analysis is not just about finding one simple answer. A stronger analysis requires cleaning data carefully, comparing multiple variables, checking limitations, and avoiding causal claims when the data only supports association.
