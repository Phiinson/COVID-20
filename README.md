# Unified COVID-19 Dataset
[![Copyright: © 2020 JHU)](https://img.shields.io/badge/Copyright-%C2%A9%202020%20JHU-blue.svg)](https://pages.jh.edu/~hbadr1)
[![Credits: NASA](https://img.shields.io/badge/Credits-NASA-blue.svg)](#Credits)
[![Citation: Badr et. al 2020](https://img.shields.io/badge/Citation-Badr%20et%20al.%202020-blue.svg)](#Citation)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![GitHub Commit](https://img.shields.io/github/last-commit/hsbadr/COVID-19)](https://github.com/hsbadr/COVID-19/commits/master)

This is an all-in-one unified COVID-19 dataset to fulfil the following objectives:
  * Mapping all geographic units globally into a unique standardized ID.
  * Standardizing administrative names and codes at all levels.
  * Standardizing dates, data types, and formats.
  * Unifying variable names, types, and categories.
  * Merging data from all credible sources at all levels.
  * Cleaning the data and fixing confusing entries.
  * Integrating an augmented version from all sources (future releases).
  * Optimizing the data for machine learning applications.

## Geographic ID

<img src="https://pages.jh.edu/~hbadr1/files/COVID-19_ID.svg#2" title="Geographic ID for the Unified COVID-19 Dataset" alt="COVID-19 ID" style="display: block; margin: auto;" />

## Lookup Table

|     Column         |    Type    |              Description            |
|:------------------:|:----------:|:------------------------------------|
| **ID**             | Charachter | Geographic ID, unique identifier (described above) |
| **NameID**         | Charachter | Full combined name of geographic unit, unique ID |
| **Admin0**         | Charachter | Standard name of administrative level 0 (countries) |
| **Admin1**         | Charachter | Standard name of administrative level 1 (provinces/states) |
| **Admin2**         | Charachter | Standard name of administrative level 2 (subregions/counties) |
| **Admin3**         | Charachter | Standard name of administrative level 3 (districts/ZIP code areas) |
| **ISO1_3N**        | Charachter | ISO 3166-1 numeric code, 3-digit, administrative level 0 (countries) |
| **ISO1_3C**        | Charachter | ISO 3166-1 alpha-3 code, 3-letter, administrative level 0 (countries) |
| **ISO1_2C**        | Charachter | ISO 3166-1 alpha-2 code, 2-letter, administrative level 0 (countries) |
| **ISO2**           | Charachter | ISO 3166-2 code, principal subdivisions (provinces/states) |
| **ISO2_UID**       | Charachter | ISO 3166-2 code, principal subdivisions (provinces/states), full/unique |
| **FIPS**           | Charachter | Federal Information Processing Standard (FIPS, United States) |
| **NUTS**           | Charachter | Nomenclature of Territorial Units for Statistics (NUTS, Europe) |
| **AGS**            | Charachter | Official municipality key / Amtlicher Gemeindeschlüssel (AGS, German regions only) |
| **ZTCA**           | Charachter | ZIP Code Tabulation Area (ZCTA) |
| **Longitude**      | Double     | Geographic coordinate (centroid), east–west |
| **Latitude**       | Double     | Geographic coordinate (centroid), north–south |
| **Population**     | Integer    | Population of each geographic unit |

## Data Structure

|     Column         |    Type    |              Description            |
|:------------------:|:----------:|:------------------------------------|
| **ID**             | Charachter | Geographic ID, unique identifier (described above) |
| **Date**           | Date       | Date of data record |
| **Cases**          | Integer    | Number of cumulative cases |
| **Cases_New**      | Integer    | Number of new daily cases |
| **Type**           | Charachter | Type of the reported cases |
| **Age**            | Charachter | Age group of the reported cases |
| **Sex**            | Charachter | Sex/gender of the reported cases |
| **Source**         | Charachter | Source of the data: CTP, JHU, NYT, DPC, RKI |
| **Level**          | Charachter | Geographic level: County, Jurisdiction, State, Province, Cruise Ship, Country |

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
| **DPC** | [Italian Civil Protection Department](https://github.com/pcm-dpc/COVID-19) | NUTS 0-3, Italy |
| **RKI** | [Robert Koch-Institut, Germany](https://npgeo-corona-npgeo-de.hub.arcgis.com/datasets/dd4580c810204019a7b8eb3e0b329dd6_0) | NUTS 0-3, Germany |

## Credits

This work is supported by NASA Health & Air Quality project `80NSSC18K0327`, under a COVID-19 supplement.

## Citation

To cite this dataset:

> Badr, H. S., **2020**: Unified COVID-19 Dataset. _GitHub_, `https://github.com/hsbadr/COVID-19`.
