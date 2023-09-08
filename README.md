# Why the Federal Reserve May Continue to Raise Interest Rates in 2023 :chart_with_downwards_trend:

## Introduction

**"Will the Federal Reserve raise interest rates again this year?"** is the question I have been asked more than I can remember from both friends and clients year-round. 2022-2023 has been an absurd period in the world of finance as the Fed went from holding the federal funds rate at around zero as recently as the first quarter of 2022 to increasing the federal fund rate a total of 11 times; making it the highest level in over 22 years.

Federal Reserve officials in recent months emphasized the importance of how their decisions will be increasingly data-dependent and noted the significance of analyzing incoming data to determine monetary policy changes moving forward. So I wanted to explore deeper into the past U.S. Macroeconomic data to help better understand the present and prepare for the future amid economic uncertainty. 

## Questions I wanted to answer:

- What are the leading economic indicators to analyze the overall strength of the U.S. economy? What were they like during the past recessions?
- What kind of consequences would higher interest rates have on the U.S. economy and what would that mean for investors?
- Is the U.S. economy heading into a recession or will there be a "soft landing"?
- Why is the Federal Reserve targeting an inflation rate of 2%?
- Will the Federal Reserve raise interest rates of another 25 basis points? 

**Why I created this project?**
- Since beginning of the year, I realized that most people were very optimistic about the economy and said the Fed would no longer have the reason to raise nominal interest rates. Market "experts" even stated that the Fed would in fact start cutting interest rates towards the end of 2023.
- However, that was not the case and inflation started to creep up even higher. People now believe interest rates will remain high until 2024 due to inflation, but have not explained the kind of consequences that may have on the economy. So I wanted to share my research and personal opinion with everyone to use as a resource. :books:

## U.S. Macroeconomic Data

For this project, we are analyzing the [U.S. Macroeconomic data](https://www.statsmodels.org/stable/datasets/generated/macrodata.html) provided on statsmodels and [kaggle](https://www.kaggle.com/datasets/nicolasgonzalezmunoz/world-bank-world-development-indicators) using data that's been collected from [The World Bank Group](https://www.worldbank.org/en/about/legal/terms-of-use-for-datasets).

The dataset has been uploaded [here](https://github.com/tylerchg/Project_1). Please see below the summarized information of the datasets:

**Statsmodels**
- Year - 1959Q1-2009Q3 
- Quarter - 1-4
- Realgdp - Real gross domestic product (Bil. of chained 2005 US$, seasonally adjusted annual rate)
- Realcons - Real personal consumption expenditures (Bil. of chained 2005 US$, seasonally adjusted annual rate)
- Realinv - Real gross private domestic investment (Bil. of chained 2005 US$, seasonally adjusted annual rate)
- Cpi - End of the quarter consumer price index for all urban consumers: all items (1982-84 = 100, seasonally adjusted)
- Unemp - Seasonally adjusted unemployment rate (%)
- Infl - Inflation rate (ln(cpi_{t}/cpi_{t-1}) * 400)
- Realint - Real interest rate (tbilrate - infl)

**The World Bank Group**
- Country - The country or geographic region (United States)
- Date - Date of the measurement (1960-2022)
- Inflation_annual% - Inflation, consumer prices, as annual %
- Real_interest_rate - Real interest rate (%)
- Risk_premium_on_lending - Risk premium on lending (lending rate minus treasury bill rate, %)
- Doing_business - Ease of doing business score (0 = lowest performance to 100 = best performance)
- Gdp_current_us - GDP (current US$)
- Gini_index - Gini index

***

## Table of Contents

:pushpin: [Assessing Data](#assessing-data)
:pushpin:
:pushpin:
:pushpin:

***

## Assessing Data

We import the required libraries and load the statsmodels dataset.
- Pandas - Data manipulation
- Numpy - Data arrays
- Matplotlib & Seaborn - Data visualisation

(To be continued)