# Tables schemas

## Index

### Schema
| Name | Type | Description | Example |
| ---- | ---- | ----------- | ------- |
| **location_key** | `string` | Identifying the region | US_CA_06001 |
| **country_code** | `string` | 2-letter code of the country | US |
| **country_name** | `string` | Name of the country, subject to change | United States of America |
| **subregion1_name** | `string` | Name of the subregion, subject to change | California |
| **subregion2_name** | `string` | Name of the county (or local equivalent), subject to change | Alameda County |

### URL
This table can be found at the following URLs:
* [age.csv](https://github.com/chica-94/COVID19-Data-Analysis/tables/)

### Data source
| Data | Source | 
| ---- | ------ | 
| Google Covid-19 Open Data (By-Age) | (https://storage.googleapis.com/covid19-open-data/v3/by-age.csv) |



## Hospitalizations

### Schema
| Name | Type | Description | Example |
| ---- | ---- | ----------- | ------- |
| **event_date** | `string` | ISO 8601 date (YYYY-MM-DD) of the datapoint | 2020-03-30 |
| **location_key** | `string` | Unique string identifying the region | CN_HB |
| **new_hospitalized_patients** | `integer` | Count of new cases hospitalized after positive test on this date | 34 |
| **cumulative_hospitalized_patients** | `integer` | Cumulative sum of cases hospitalized after positive test to date | 6447 |
| **new_intensive_care_patients** | `integer` | Count of new cases admitted into ICU after a positive COVID-19 test on this date | 2 |
| **cumulative_intensive_care_patients** | `integer` | Cumulative sum of cases admitted into ICU after a positive COVID-19 test to date | 133 |

### URL
This table can be found at the following URLs:
* [hospitalizations.csv](https://github.com/chica-94/COVID19-Data-Analysis/tables/)

### Data source
| Data | Source | 
| ---- | ------ | 
| Google Covid-19 Open Data (Hospitalizations) | (https://storage.googleapis.com/covid19-open-data/v3/hospitalizations.csv) |


## Health

### Schema
| Name | Type | Description | Example |
| ---- | ---- | ----------- | ------- |
| **location_key** | `string` | Identifying the region | BN |
| **adult_male_mortality_rate** | `double` | Mortality rate, adult, male (per 1,000 male adults) | 143.719 |
| **adult_female_mortality_rate** | `double` | Mortality rate, adult, female (per 1,000 male adults) | 98.803 |
| **life_expectancy** | `double` `[years]` |Average years that an individual is expected to live | 75.722 |
| **diabetes_prevalence** | `double` `[%]` | Percentage of persons with diabetes in population | 13.3 |
| **health_expenditure** | `double` `[USD]` | Health expenditure per capita | 671.4115 |
| **out_of_pocket_health_expenditure** | `double` `[USD]` | Out-of-pocket health expenditure per capita | 34.756348 |

### URL
This table can be found at the following URLs:
* [health.csv](https://github.com/chica-94/COVID19-Data-Analysis/tables/)

### Data source
| Data | Source | 
| ---- | ------ | 
| Google Covid-19 Open Data (Health) | (https://storage.googleapis.com/covid19-open-data/v3/health.csv) |



## Vaccinations

### Schema
| Name | Type | Description | Example |
| ---- | ---- | ----------- | ------- |
| **event_date** | `date` | date format (YYYY-MM-DD) | 2020-03-30 |
| **location_key** | `string` | Identifying the region | EN |
| **new_persons_fully_vaccinated** | `int` | Count of new people which have received all doses required for maximum immunity | 1924 |
| **cumulative_persons_fully_vaccinated** | `int` | Cumulative sum of people which have received all doses required for maximum immunity | 139131 |

### URL
This table can be found at the following URLs:
* [vaccinations.csv](https://github.com/chica-94/COVID19-Data-Analysis/tables/)

### Data source
| Data | Source | 
| ---- | ------ | 
| Google Covid-19 Open Data (Vaccinations) | (https://storage.googleapis.com/covid19-open-data/v3/vaccinations.csv) |



## Demographics

### Schema
| Name | Type | Description | Example |
| ---- | ---- | ----------- | ------- |
| **location_key** | `string` | Unique string identifying the region | KR |
| **population** | `int` | Total count of humans | 51606633 |
| **population_male** | `int` | Total count of males | 25846211 |
| **population_female** | `int` | Total count of females | 25760422 |
| **population_age_00_09** | `int` | Estimated population between the ages of 0 and 9| 42038247 |
| **population_age_10_19** | `int` | Estimated population between the ages of 10 and 19| 42038247 |
| **population_age_20_29** | `int` | Estimated population between the ages of 20 and 29| 42038247 |
| **population_age_30_39** | `int` | Estimated population between the ages of 30 and 39| 42038247 |
| **population_age_40_49** | `int` | Estimated population between the ages of 40 and 49| 42038247 |
| **population_age_50_59** | `int` | Estimated population between the ages of 50 and 59| 42038247 |
| **population_age_60_69** | `int` | Estimated population between the ages of 60 and 69| 42038247 |
| **population_age_70_79** | `int` | Estimated population between the ages of 70 and 79| 42038247 |
| **population_age_80_and_older** | `int` | Estimated population over the age of 80 | 477081 |

### URL
This table can be found at the following URLs:
* [demographics.csv](https://github.com/chica-94/COVID19-Data-Analysis/tables/)

### Data source
| Data | Source | 
| ---- | ------ | 
| Google Covid-19 Open Data (Demographics) | (https://storage.googleapis.com/covid19-open-data/v3/demographics.csv) |



## Geography

### Schema
| Name | Type | Description | Example |
| ---- | ---- | ----------- | ------- |
| **location_key** | `string` | Identifying the region | CN |
| **latitude** | `double` | Floating point representing the geographic coordinate | 30.9756 |
| **longitude** | `double` | Floating point representing the geographic coordinate | 112.2707 |

### URL
This table can be found at the following URLs:
* [geography.csv](https://github.com/chica-94/COVID19-Data-Analysis/tables/)

### Data source
| Data | Source | 
| ---- | ------ | 
| Google Covid-19 Open Data (Geography) | (https://storage.googleapis.com/covid19-open-data/v3/geography.csv) |



## Epidemiology

### Schema
| Name | Type | Description | Example |
| ---- | ---- | ----------- | ------- |
| **event_date** | `string` | ISO 8601 date (YYYY-MM-DD) of the datapoint | 2020-03-30 |
| **location_key** | `string` | Unique string identifying the region | CN_HB |
| **new_confirmed** | `int` | Count of new cases confirmed after positive test on this date | 34 |
| **cumulative_confirmed** | `int` | Cumulative sum of cases confirmed after positive test to date | 6447 |
| **new_deceased** | `int` | Count of new deaths from a positive COVID-19 case on this date | 2 |
| **cumulative_deceased>** | `int` | Cumulative sum of deaths from a positive COVID-19 case to date | 133 |
| **new_recovered** | `int` | Count of new recoveries from a positive COVID-19 case on this date | 13 |
| **cumulative_recovered** | `int` | Cumulative sum of recoveries from a positive COVID-19 case to date | 133 |

### URL
This table can be found at the following URLs:
* [epidemiology.csv](https://github.com/chica-94/COVID19-Data-Analysis/tables/)

### Data source
| Data | Source | 
| ---- | ------ | 
| Google Covid-19 Open Data (Epidemiology) | (https://storage.googleapis.com/covid19-open-data/v3/epidemiology.csv) |



## Gender

### Schema
| Name | Type | Description | Example |
| ---- | ---- | ----------- | ------- |
| **event_date** | `date` | date format (YYYY-MM-DD) | 2020-03-30 |
| **location_key** | `string` | Identifying the region | AR |
| **new_deceased_sex_male** | `int` | Value of newly deceased of that date for male individuals | 87 |
| **cumulative_deceased_sex_male** * | `int` | Value of cumulative deceased for male individuals | 68 |
| **new_deceased_sex_female**  | `int` | Value of newly deceased of that date for female individuals | 87 |
| **cumulative_deceased_sex_female** * | `int` | Value of cumulative deceased for female individuals | 68 |
| **new_recovered_sex_male**  | `int` | Value of newly recovered patients of that date for male individuals | 87 |
| **cumulative_recovered_sex_male** * | `int` | Value of cumulative recovered for male individuals | 68 |
| **new_recovered_sex_female**  | `int` | Value of newly recovered patients of that date for female individuals | 87 |
| **cumulative_recovered_sex_female** ** | `int` | Value of cumulative recovered for female individuals | 68 |

### URL
This table can be found at the following URLs:
* [age.csv](https://github.com/chica-94/COVID19-Data-Analysis/tables/)

### Data source
| Data | Source | 
| ---- | ------ | 
| Google Covid-19 Open Data (By Sex) | (https://storage.googleapis.com/covid19-open-data/v3/by-sex.csv) |



## Age


### Schema
| Name | Type | Description | Example |
| ---- | ---- | ----------- | ------- |
| **event_date** | `date` | date format (YYYY-MM-DD) | 2020-03-30 |
| **location_key** | `string` | Identifying the region | FR |
| **new_recovered_age_0-9** | `int` | Value of newly recovered patients of that date for ages 0-9 | 3 |
| **new_recovered_age_10-19** | `int` | Value of newly recovered patients of that date for ages 10-19  | 3 |
| **new_recovered_age_20-29** | `int` | Value of newly recovered patients of that date for ages 20-29 | 3 |
| **new_recovered_age_30-39** | `int` | Value of newly recovered patients of that date for ages 30-39 | 3 |
| **new_recovered_age_40-49** | `int` | Value of newly recovered patients of that date for ages 40-49 | 3 |
| **new_recovered_age_50-59** | `int` | Value of newly recovered patients of that date for ages 50-59 | 3 |
| **new_recovered_age_60-69** | `int` | Value of newly recovered patients of that date for ages 60-69 | 3 |
| **new_recovered_age_70-79** | `int` | Value of newly recovered patients of that date for ages 70-79 | 3 |
| **new_recovered_age_80-89** | `int` | Value of newly recovered patients of that date for ages 80-89 | 3 |
| **new_recovered_age_90-99** | `int` | Value of newly recovered patients of that date for ages 90-99 | 3 |
| **cumulative_recovered_age_0-9** | `int` | Total value of patients recovered for ages 0-9 | 1037 |
| **cumulative_recovered_age_10-19** | `int` | Total value of patients recovered for ages 10-19 | 1037 |
| **cumulative_recovered_age_20-29** | `int` | Total value of patients recovered for ages 20-29 | 1037 |
| **cumulative_recovered_age_30-39** | `int` | Total value of patients recovered for ages 30-39 | 1037 |
| **cumulative_recovered_age_40-49** | `int` | Total value of patients recovered for ages 40-49 | 1037 |
| **cumulative_recovered_age_50-59** | `int` | Total value of patients recovered for ages 50-59 | 1037 |
| **cumulative_recovered_age_60-69** | `int` | Total value of patients recovered for ages 60-69 | 1037 |
| **cumulative_recovered_age_70-79** | `int` | Total value of patients recovered for ages 70-79 | 1037 |
| **cumulative_recovered_age_80-89** | `int` | Total value of patients recovered for ages 80-89 | 1037 |
| **cumulative_recovered_age_90-99** | `int` | Total value of patients recovered for ages 90-99 | 1037 |


### URL
This table can be found at the following URLs:
* [age.csv](https://github.com/chica-94/COVID19-Data-Analysis/tables/)

### Data source

| Data | Source | 
| ---- | ------ | 
| Google Covid-19 Open Data (By Age) | (https://storage.googleapis.com/covid19-open-data/v3/by-age.csv) |