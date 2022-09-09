# Determinants of U.S. County-Level COVID-19 Mortality

This is the public-facing repository for our summer 2022 Stanford Data Science for Social Good project, Determinants of U.S. County-Level COVID-19 Mortality. The [full repository](https://github.com/StanfordDataScience/dssg_covid_mortality) will be available upon full project completion, but this partial repository is meant to share with interested partners for the 2022 Data Science for Social Good Conference.

Below are project details: 

## Team members:

-   **Jiancheng Ge**
-   [**Charles Hendrickson**](https://charleshendrickson.github.io)
-   [**Scout Leonard**](https://scoutcleonard.github.io)

## Technical Mentor:

- Min Woo Sun (Stanford University)

## Faculty Mentors: 

- Dr. Robert Tibshirani (Stanford University)
- Dr. Balasubramanian Narashiman (Stanford University)

## Project Significance and Summary: 

Since the start of the COVID-19 pandemic, more than one million Americans have died from COVID-19 (CDC 2020). These deaths have been tracked and reported using death certificate cause of death claims. This method of tracking COVID-19 deaths can misrepresent the true mortality burden of the pandemic for a variety of reasons. Reported COVID-19 deaths may not reflect true mortality burdens because COVID-19 testing has not been accessible for the duration of the pandemic. There are also indirect COVID-19 deaths that contribute to the mortality burden of a pandemic, including strained healthcare systems (Ackley et al. 2022).

Estimating excess mortality has been utilized as a more achievable way to capture the full mortality burden of the pandemic (Ackley et al. 2022, Knuston et al. n.d.). Excess death describes the difference between all cause mortality, the reported death from all causes for a given period of time, and expected mortality, the expected amount of death based on historic death rates.

In this project, we model the COVID-19 excess mortality rate in the United States at the county level and analyze the effect of socioeconomic, health, vaccination, and policy factors on estimated excess mortality for 2020-2021 using statistical learning models. This study will help elucidate the factors contributing to the U.S. county-level excess mortality rate and guide policy-makers in U.S. counties in improving their response to pandemics, with the goal of ultimately reducing the number of American deaths by guiding effective and equitable policy interventions. Our study utilizes open, reproducible, and rigorous science and can be used as a template for further research on the determinants of COVID-19 mortality.

It is noteworthy that previous studies have investigated the effect of determinants of COVID-19 mortality, but have focused solely on confirmed COVID-19 deaths (Miller et al. 2020, Squalli et al. 2020). Instead, our study models excess deaths, which is widely considered a more objective indicator of the COVID-19 death toll. Furthermore, there has not been a holistic analysis including variables describing policies, such as stay at home orders, mask mandates, and COVID-19 vaccination rate.

## Goal

The goal of this project was to build a model which generates reliable estimates of excess mortality at the U.S. county level for 2020 and 2021 using publicly available data. Using these excess mortality estimates, the fellows built models to analyze the effect that various socioeconomic, health, vaccination, and policy factors have on excess death at the U.S. county level.

<p align="center">
  <img src="https://github.com/StanfordDataScience/dssg_covid_mortality/blob/main/plan.png" width="800" height="450" />
</p>

------------------------------------------------------------------------

## Data sources

All data used in this project are from open source repositories. All datasets were manually downloaded.

For datasets that were too large to for this GitHub repository, details about how and when the dataset was access are available in the project data directory, [`analysis/County/data/raw_data/Data Download Documentation.txt`](https://github.com/StanfordDataScience/dssg_covid_mortality/blob/main/analysis/County/data/raw_data/Data%20Download%20Documentation.txt). 

### Phase I Analysis: Estimating Excess Death for U.S. Counties

-   [National Center for Health Statistics Mortality Data on CDC WONDER](https://wonder.cdc.gov/mcd.html)

### Phase II Analysis: COVID-19 Mortality Feature Importance

#### Vaccination Data:

-   [County-Level Vaccination Data](https://data.cdc.gov/Vaccinations/COVID-19-Vaccinations-in-the-United-States-County/8xkx-amqh)
-   [Massachusetts COVID-19 Vaccination Data for missing values in Barnstable](https://www.mass.gov/info-details/archive-of-covid-19-vaccination-reports#july-2022-)
-   [Hawaii COVID-19 Vaccination Data for missing values in all Hawaii counties](https://health.hawaii.gov/coronavirusdisease2019/)

#### Policy Data:

-   [health.gov state and policy orders](https://healthdata.gov/dataset/COVID-19-State-and-County-Policy-Orders/gyqz-9u7n)

#### Intrinsic Data:

-   [University of Wisconsin County Health Rankings and Roadmaps for 2020 and 2021](https://www.countyhealthrankings.org/explore-health-rankings/rankings-data-documentation)
