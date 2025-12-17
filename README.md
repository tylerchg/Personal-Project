# Why the Federal Reserve May Continue to Raise Interest Rates :chart_with_downwards_trend:

## Introduction

**"Will the Federal Reserve raise interest rates again this year?"** is the question I have been asked more than I can remember from both friends and clients year-round. 2022-2023 has been an absurd period in the world of finance as the Fed went from holding the federal funds rate at near zero as recently as the first quarter of 2022 to increasing the rate a total of 11 times; making it the highest level in over 22 years.

Federal Reserve officials in recent months emphasized the importance of how their decisions will be increasingly data-dependent and noted the significance of analyzing incoming data to determine monetary policy changes moving forward. So I wanted to explore deeper into the past U.S. macroeconomic data to help better understand the present and prepare for the future amid economic uncertainty. 

***

## Table of Contents

:pushpin: [Assessing Data](#assessing-data)

:pushpin: [Data Wrangling](#data_wranglings)

:pushpin: [Data Analysis and Visualization](#data_analysis_and_visualization)

:pushpin: [Reference](#reference)

***

## Questions

- Does higher real interest rates result in higher unemployment rates?
- What were the unemployment and real interest rates like when inflation rates were less than or equal to 2%?
- When did the U.S. economy (in years) have the highest unemployment when inflation rates were less than or equal to 2%?
- When did the U.S. economy (in years) have the highest inflation rates?

**Why I created this project?**

- Since beginning of the year, I realized that most people were very optimistic about the economy and said the Fed would no longer have the reason to raise nominal interest rates. Market experts even stated that the Fed would in fact start cutting interest rates towards the end of 2023.
- However, that has not the case and inflation started to creep up even higher. People now believe interest rates will remain high until 2024 due to inflation, but have not explained the kind of consequences that may have on the economy. So I wanted to share my research and personal opinion with everyone to use as a resource.

## Required Libraries and Datasets

- Pandas - Data manipulation
- NumPy - Data arrays
- Matplotlib & Seaborn - Data visualisation

```python
# Importing libraries
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

# Loading csv file (Statsmodels)
data = pd.read_csv('macrodata.csv')

# Loading csv file (The World Bank Group)
data2 = pd.read_csv('inflation_interest_unemployment.csv')
```

## U.S. Macroeconomic Data

For this project, I will be analyzing the [U.S. macroeconomic data](https://www.statsmodels.org/stable/datasets/generated/macrodata.html) provided on statsmodels and [kaggle](https://www.kaggle.com/datasets/prasertk/inflation-interest-and-unemployment-rate) using data that's been collected from [The World Bank Group](https://www.worldbank.org/en/about/legal/terms-of-use-for-datasets).

The project and datasets have been uploaded [here](https://github.com/tylerchg/Personal-Project/tree/main/U.S.%20Macroeconomic%20Data%20Analysis). Please see below the summarized information:

**Statsmodels**
- `Year` - 1959Q1-2009Q3 
- `Quarter` - 1-4
- `Realgdp` - Real gross domestic product (Bil. of chained 2005 US$, seasonally adjusted annual rate)
- `Realcons` - Real personal consumption expenditures (Bil. of chained 2005 US$, seasonally adjusted annual rate)
- `Realinv` - Real gross private domestic investment (Bil. of chained 2005 US$, seasonally adjusted annual rate)
- `Cpi` - End of the quarter consumer price index for all urban consumers: all items (1982-84 = 100, seasonally adjusted)
- `Unemp` - Seasonally adjusted unemployment rate (%)
- `Infl` - Inflation rate (ln(cpi_{t}/cpi_{t-1}) * 400)
- `Realint` - Real interest rate (tbilrate - infl)

**The World Bank Group**
- `Country` - The country or geographic region (United States)
- `Year` - Date of the measurement (1970-2021)
- `Inflation, consumer prices (annual %)` - Inflation, consumer prices, as annual %
- `Inflation, GDP deflator (annual %)` - Inflation, GDP deflator, as annual %
- `Real interest rate (%)` - Real interest rate
- `Unemployment, total (% of total labor force) (national estimate)` - Unemployment % of total labor force
- `Unemployment, total (% of total labor force) (modeled ILO estimate)` - Unemployment % of total labor force


## Assessing Data

Preparing datasets:
- How many samples (rows/observations) and columns are in both datasets?
- Are there any duplicates?
- What are the data types?
- Are there any missing values?
- What are the unique values and the count?

## Data Wrangling

Cleaning datasets:
- Creating a time based index.
- Replacing an existing index.
- Specifying a new index.
- Dropping extraneous columns.
- Conforming to the column index specified.
- Stacking to create a series (if needed).

## Data Analysis and Visualization

Filtering and exploring datasets:
- Descriptive statistical analysis.
- Exploring leading economic indicators to analyze the overall strength of the U.S. economy.
- Periods where inflation rates were less than or equal to 2%.
- Sorting by unemployment rate to analyze any correlation with inflation.
- Analyzing the importance of real interest rates during past recessions.
- Bivariate and multivariate plots.
- Pair-wise plots for multiple numeric data variables.
- Fitting basic statistical models.
- Exporting filtered data into a new csv file.

## Reference :books:

- [Statsmodels](https://www.statsmodels.org/stable/datasets/generated/macrodata.html)
- [Kaggle](https://www.kaggle.com/datasets/prasertk/inflation-interest-and-unemployment-rate)
- [The World Bank](https://www.worldbank.org/en/about/legal/terms-of-use-for-datasets)
- [Investopedia: Leading Indicators](https://www.investopedia.com/terms/l/leadingindicator.asp)
- [Investopedia: Top 10 U.S. Economic Indicators](https://www.investopedia.com/articles/personal-finance/020215/top-ten-us-economic-indicators.asp)
- [Investopedia: US Recessions Throughout History](https://www.investopedia.com/articles/economics/08/past-recessions.asp)
- [Investopedia: Taylor Rule Definition](https://www.investopedia.com/terms/t/taylorsrule.asp)
- [Northwestern Mutual: What's the Real Interest Rate and Why Does It Matter?](https://www.northwesternmutual.com/life-and-money/whats-the-real-interest-rate-and-why-does-it-matter/)
- [University of Chicago (Booth): What Target Should the Fed Be Shooting At?](https://www.chicagobooth.edu/review/what-target-should-fed-be-shooting#:~:text=The%20traditional%20view%20is%20that,are%20rethinking%20this%20conventional%20wisdom.)
- [Board of Governors of the Federal Reserve System](https://www.federalreserve.gov/faqs/economy_14400.htm)
- [TheStreet: What Is a Real Interest Rate?](https://www.thestreet.com/dictionary/r/real-interest-rate)
- [Investopedia: US Recessions Throughout History](https://www.investopedia.com/articles/economics/08/past-recessions.asp)


## License
This work is licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0).

## Disclaimer
This repository is provided for educational and informational purposes only and does not constitute investment, legal, or financial advice.
