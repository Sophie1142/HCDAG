# HCDAG Economics Think Tank
## Overview
Team repository for Harvard College Data Analytics Group (HCDAG) Economics Think Tank project on coronavirus, Summer 2020.

**Project Leaders:** Sophie E. and Meghan T.

**Researchers:** Vivian Z. and Tivas G.

**Supervisor:** Kelsey W.

**Article:** [TODO: insert link]

**Contact Us:**

We welcome your thoughts and questions!

* Organization: contact@harvardanalytics.org

* Project Leads: sedouard@college.harvard.edu & mturner@college.harvard.edu


**Terms of Use:**

Please attribute any data and/or ideas from our article...
TODO (see OpportunityInsights & John Hopkins repo's for inspiration)

## Data Sources

### General

Geographic identification files at the state and county level were acquired from the Opportunity Insights Econometric Tracker [public data repository](https://github.com/OpportunityInsights/EconomicTracker). 

* View their paper here: (https://opportunityinsights.org/wp-content/uploads/2020/05/tracker_paper.pdf)

* View their Economic Tracker website: https://tracktherecovery.org/


File Description:
"...We have [2] files, **GeoIDs – State** and **GeoIDs – County** ..., that provide information on geographic crosswalks and aggregation. These can be merged to any file sharing the same geographic level of aggregation using the geographic identifier. Additionally, **GeoIDs – County** indicates the commuting zone (CZ) and state that each county belongs to. The City-level data (listed under "Metro" on the tracker site) associates the largest cities in the United States with a representative county one-to-one (except in the case of New York City which includes the 5 boroughs).

A description of the columns in each file follows.

#### GeoIDs - State.csv

Geographic identifier: `statefips`

- `statename`: The name of the state.
- `stateabbrev`: The 2-letter state abbreviation.
- `state_pop2019`: The population of the state in 2019, from Census Bureau estimates.

#### GeoIDs - County.csv

Geographic identifier: `countyfips`

- `countyname`: The name of the county.
- `cz`: The numeric identifier of the commuting zone (CZ) in which the county is contained.
- `czname`: The name of the commuting zone (CZ) in which the county is contained.
- `statename`: The name of the state in which the county is contained.
- `statefips`: The fips code of the state in which the county is contained.
- `stateabbrev`: The 2-letter abbreviation of the state in which the county is contained.
- `county_pop2019`: The population of the county in 2019, from Census Bureau estimates.


## Coronavirus Data

TO DO: Generate rates for TOTAL confirmed and deaths

**Data Source:** County-level time series data on US coronavirus infections and deaths from January 21 through August 4, 2020 were acquired from the COVID-19 Data Repository by the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University. View their Github repository for more in-depth documentation at https://github.com/CSSEGISandData/COVID-19. 

* **Important Note:** Due to the nature of our analysis, data is up to date through August 4th.

In addition, we used the the U.S. Census Bureau 2019 Population Estimates [dataset](https://www.census.gov/data/datasets/time-series/demo/popest/2010s-counties-total.html) to convert coronavirus stats into rates so that counties different population sizes could be compared.

All coronavirus datasets contain the following variables:
* `UID`: Unique ID generated by Johns Hopkins team
* `FIPS`: County FIPS code
* `County`: County name
* `State`: State name
* `Combined_Key`: County, State

In addition, biweekly **confirmed/deaths** CSV files report coronavirus statistics in absolute numbers and contain the following variables:
* `2/5/20`: Total new COVID-19 **confirmed cases/deaths** in the 2 week period from 1/22/20 to 2/5/2020
* `2/19/20`: Total new COVID-19 **confirmed cases/deaths** in the 2 week period from 2/5/2020 to 2/19/2020
* And so on until `8/5/2020`

Biweekly confirmed/deaths **rate** files report the correpsonding coronavirus statistic as a rate of per 100,000 people and contain the same date intervals as the above biweekly files. Thus, in these files, the variables are as follows:
* `2/5/20`: Total new COVID-19 confirmed cases/deaths **per 100,000 people** in the 2 week period from 1/22/20 to 2/5/2020
* `2/19/20`: Total new COVID-19 confirmed cases/deaths **per 100,000 people**in the 2 week period from 2/5/2020 to 2/19/2020
* And so on until `8/5/2020`


The **monthly** files are set up similarly but using 4-week time intervals.

## Demographic and Economic Data

County-level demographic and economic data (median household income, racial data etc) were acquired from the 2018 American Community Survey ([ACS](https://www.census.gov/programs-surveys/acs)) 5-Year Profile data.

VIVIAN, TODO (if needed)

## Unemployment Data

County-level, monthly unemployment data through MAY/JUNE 2020 was acquired from the US Bureau of Labor Statistics (BLS) Local Areas Unemployment Statistics ([LAUS](https://www.bls.gov/lau/#news)). 

## Political Data
TIVAS, TODO

## State Lockdowns Data

School closings: https://www.edweek.org/ew/section/multimedia/map-coronavirus-and-school-closures.html


#### Sources of Inspiration/Other
* [TIME - These Graphs Show How COVID-19 Is Ravaging NYC's LICs](https://time.com/5821212/coronavirus-low-income-communities/)
* [USA Today - We looked at coronavirus in 8,500 ZIP codes across America. Here's what we found](https://www.usatoday.com/in-depth/graphics/2020/06/30/maps-covid-19-rich-and-poor-neighborhoods-show-big-disparities/3257615001/)
* [KFF - LICs Communities of Color at Higher Risk of Serious Illness if Infected](https://www.kff.org/coronavirus-covid-19/issue-brief/low-income-and-communities-of-color-at-higher-risk-of-serious-illness-if-infected-with-coronavirus/)
* Harvard Professor Chetty and the team at Opportunity Insights (https://tracktherecovery.org)

#### Acknowledgements
* Preceptor David Kane
* Professor Chris Foote


