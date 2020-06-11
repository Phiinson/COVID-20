# Unified COVID-19 Dataset
[![Copyright © 2020 Johns Hopkins University (JHU)](https://img.shields.io/badge/Copyright-%C2%A9%202020%20Johns%20Hopkins%20University%20%28JHU%29-blue.svg)](https://pages.jh.edu/~hbadr1)
[![Citation: Badr et. al 2020](https://img.shields.io/badge/Citation-Badr%20et%20al.%202020-blue.svg)](#Citation)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![GitHub Commit](https://img.shields.io/github/last-commit/hsbadr/COVID-19)](https://github.com/hsbadr/COVID-19/commits/master)

This is an all-in-one unified COVID-19 dataset to fulfil the following objectives:
  * Merging data from all credible sources at all levels
  * Unifying variable names, types, and categories
  * Standardizing Country/Province/State/County names
  * Standardizing Country/Province/State/County codes
  * Standardizing dates and data types/formats
  * Cleaning the data and fixing confusing entries
  * Optimizing the data for machine learning applications

## Data Structure

|     Column         |    Type    |              Description             |
|:------------------:|:----------:|:------------------------------------|
| **Date**           | Date       | Date of data record |
| **Year**           | Integer    | Year of data record |
| **Month**          | Integer    | Month of data record |
| **Day**            | Integer    | Day of data record |
| **DoW**            | Charachter | Day of the week |
| **Cases**          | Integer    | Number of cumulative cases |
| **Cases_New**      | Integer    | Number of new daily cases |
| **Type**           | Charachter | Type of the reported cases |
| **Source**         | Charachter | Source of the data: CTP, JHU, NYT, DPC, RKI |
| **Level**          | Charachter | Geographic level: County, Jurisdiction, State, Province, Cruise Ship, Country |
| **Longitude**      | Double     | Geographic coordinate (centroid), east–west |
| **Latitude**       | Double     | Geographic coordinate (centroid), north–south |
| **Population**     | Integer    | Population of each geographic unit |
| **ISO3166_1_3N**   | Charachter | ISO 3166-1 numeric code, 3-digit, country/region |
| **ISO3166_1_3C**   | Charachter | ISO 3166-1 alpha-3 code, 3-letter, country/region |
| **ISO3166_1_2C**   | Charachter | ISO 3166-1 alpha-2 code, 3-letter, country/region |
| **ISO3166_2**      | Charachter | ISO 3166-2 code, province/state |
| **ISO3166_2_UID**  | Charachter | ISO 3166-2 code, province/state, full/unique |
| **NUTS**           | Charachter | Nomenclature of Territorial Units for Statistics (NUTS), Europe |
| **FIPS**           | Charachter | Federal Information Processing Standard Publication, United States |
| **County**         | Charachter | Standard county name |
| **Province_State** | Charachter | Standard province/state name |
| **Country_Region** | Charachter | Standard country/region name |
| **Full_Name**      | Charachter | Full combined name of geographic unit, unique ID |

## Case Types

|        Type          |    Description   |
|:--------------------:|:-----------------|
| **Active**           | Active cases |
| **Confirmed**        | Confimed cases |
| **Deaths**           | Deaths |
| **Home_Isolation**   | Home isolation |
| **Hospitalized**     | Total hospitalized cases excluding intensive care units |
| **Hospitalized_Now** | Currently hospitalized cases excluding intensive care units |
| **Hospitalized_Sym** | Symptomatic hospitalized cases excluding intensive care units |
| **ICU**              | Total cases in intensive care units |
| **ICU_Now**          | Currently in intensive care units |
| **Negative**         | Negative tests |
| **Pending**          | Pending tests |
| **Positive**         | Positive tests |
| **Recovered**        | Recovered cases |
| **Tested**           | Cases tested = Tests - Pending |
| **Tests**            | Total performed tests |
| **Ventilator**       | Total cases receiving mechanical ventilation |
| **Ventilator_Now**   | Currently receiving mechanical ventilation |


## Data Sources

| Source  |    Description   |    Level    |
|:-------:|:-----------------|:------------|
| **JHU** | [The Johns Hopkins University Center for Systems Science and Engineering](https://github.com/CSSEGISandData/COVID-19) | Global & County/State, United States |
| **CTP** | [The COVID Tracking Project](https://covidtracking.com) | State, United States |
| **NYT** | [The New York Times](https://github.com/nytimes/covid-19-data) | County/State, United States |
| **DPC** | [Italian Civil Protection Department](https://github.com/pcm-dpc/COVID-19) | NUTS3/NUTS2, Italy |
| **RKI** | [Robert Koch-Institut, Germany](https://npgeo-corona-npgeo-de.hub.arcgis.com/datasets/dd4580c810204019a7b8eb3e0b329dd6_0) | NUTS3/NUTS2, Germany |

## Citation

To cite this dataset:

> Badr, H. S., **2020**: Unified COVID-19 Dataset. _GitHub_, `https://github.com/hsbadr/COVID-19`.
