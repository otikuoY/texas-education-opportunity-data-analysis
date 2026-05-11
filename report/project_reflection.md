# What I Learned from Analyzing Education Opportunity in Texas

## Why I Chose This Topic

As a private-school student in Texas, I wanted to understand educational opportunity beyond my own school experience. I was interested in how private-school access differs across communities and whether it connects to income, education level, and public-school outcomes.

## What Data I Used

I used public data from NCES, the U.S. Census ACS, and the Texas Academic Performance Reports. I cleaned and merged the datasets in Python to create county-level measures of private-school access, socioeconomic conditions, and public-school outcomes.

## What I Expected

At first, I expected median income to explain private-school access more strongly. I thought higher-income counties would clearly have more private schools per 100,000 people.

## What Surprised Me

The results were more complicated than I expected. Income alone had only a weak relationship with private-school access in larger Texas counties. Adult education level had a stronger relationship than income or poverty rate.

In Version 2, after adding public-school outcome data, I found that private-school access did not meaningfully improve the model’s ability to explain public-school CCMR rates after accounting for socioeconomic factors.

## What I Found

The project suggested that private-school access is not just an income issue. Local education level, community expectations, family preferences, urbanization, and other factors may also matter.

The analysis also showed that private-school access and public-school outcomes should not be treated as simple opposites. Counties with more private-school access did not necessarily have stronger or weaker public-school outcomes at the county level.

## What This Taught Me About Data Science

This project taught me that data science is not just about finding patterns. It also requires asking careful questions, cleaning data responsibly, testing assumptions, and avoiding causal claims when the data only supports association.

## Limitations

This analysis is correlational, not causal. County-level averages can hide important differences within counties. Public-school outcomes may also depend on factors not included in this project, such as funding, transportation, local history, school quality, and family choice.
