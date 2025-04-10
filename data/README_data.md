# 📄 **Dataset Metadata**
---
## 1. Dataset Overview
- **Title**: Worldwide Bureaucracy Indicators (WWBI) – TidyTuesday Adaptation
- **Description**:  
  Cross-national dataset on public sector employment and wages compiled by the World Bank’s Bureaucracy Lab. It provides information on public-sector employment characteristics, wages and compensations, and overall wage bills for 202 countries and territories between 2000 and 2020.

## 2. Provenance
- **Original Source**: [World Bank – Bureaucracy Lab](https://datacatalog1.worldbank.org/search/dataset/0038132/Worldwide-Bureaucracy-Indicators)  
- **Curated By**: [TidyTuesday Project](https://github.com/rfordatascience/tidytuesday/blob/main/data/2024/2024-04-30)  
- **Adaptations**:  
  - Data organized into three main files (`wwbi_data.csv`, `wwbi_series.csv`, `wwbi_country.csv`) for TidyTuesday.
  - Selected indicators for analysis: wage bill as a percentage of GDP, employment breakdown by sector, gender, and occupation level.
  
## 3. Files Included
| File Name          | Description                                                    |
|--------------------|-----------------------------------------------------------------|
| `wwbi_data.csv`     | Main data file: country code, indicator code, year, value       |
| `wwbi_series.csv`   | Mapping of indicator codes to human-readable indicator names   |
| `wwbi_country.csv`  | Country metadata including region and income group     
| `WWBI-Codebook-v3.1.pdf`  | Worldwide Bureaucracy Indicators version 3.1: Codebook and Explanatory Note     

## 4. Codebook

# `wwbi_data.csv`

|variable       |class     |description    |
|:--------------|:---------|:--------------|
|country_code   |character |3-letter ISO_3166-1 code |
|indicator_code |character |code identifying the indicator of bureaucracy |
|year           |numeric   |year of the data |
|value          |numeric   |numeric value of the data |

# `wwbi_series.csv`

|variable       |class     |description    |
|:--------------|:---------|:--------------|
|indicator_code |character |code identifying the indicator of bureaucracy |
|indicator_name |character |name of the indicator |

# `wwbi_country.csv`

|variable         |class     |description                                      |
|:----------------|:---------|:------------------------------------------------|
|country_code     |character |3-letter ISO_3166-1 code |
|short_name       |character |short or common name for the country |
|table_name       |character |more alphabetically sortable name of the country |
|long_name        |character |full name of the country |
|x2_alpha_code    |character |2-letter ISO_3166-1 code |
|currency_unit    |character |currency unit |
|special_notes    |character |special notes |
|region           |character |region |
|income_group     |character |low, lower middle, upper middle, or high income |
|wb_2_code        |character |alternate 2-letter code |
|national_accounts_base_year |integer |national accounts base year |
|national_accounts_reference_year |integer |national accounts reference year |
|sna_price_valuation |character |UN system of national accounts price valuation |
|lending_category |character |International Development Association (IDA), Interanational Bank of Reconstruction and Development (IBRD), a blend or neither |
|other_groups     |character |Heavily Indebted Poor Countries initiative (HIPC), or countries classified as the "Euro area" |
|system_of_national_accounts |integer |which System of National Accounts methodology the country uses (1968, 1993, or 2008 version) |
|balance_of_payments_manual_in_use |character |the version of the Balance of Payments Manual used by the country |
|external_debt_reporting_status |character |estimate, preliminary, or actual |
|system_of_trade  |character |Under the general system imports include goods imported for domestic consumption and imports into bonded warehouses and free trade zones. Under the special system imports comprise goods imported for domestic consumption (including transformation and repair) and withdrawals for domestic consumption from bonded warehouses and free trade zones. Goods transported through a country en route to another are excluded. |
|government_accounting_concept |character |government accounting concept |
|imf_data_dissemination_standard |character |International Monetary Fund data-dissemination standard: Special Data Dissemination Standard (SDDS, 1996, created for countries
that have or seek to have access to international markets), SDDS Plus (2012, the highest tier of data standards, intended for systemically important economies), enhanced GDDS (e-GDDS, 2015, encouraging participants to emphasize data publication) |
|latest_household_survey |character |which household survey was most recently administered |
|source_of_most_recent_income_and_expenditure_data |character |which survey serves as the basis for income and expenditure data |
|vital_registration_complete |logical |whether the vital registration is complete |
|latest_agricultural_census |integer |year of latest agricultural census |
|latest_industrial_data |integer |year of latest industrial data |
|latest_trade_data |integer |year of latest trade data |
|latest_population_census_year |integer |year of latest population census |
|latest_population_census_notes |character |notes about latest population census |

## 5. Notes on Usage
- **Skill Level Classification**:  
  Occupations are classified into high-skill (managers, professionals, technicians; ISCO-08 skill levels 3 and 4) and low-skill (clerical support workers, elementary workers; skill levels 1 and 2) categories based on ISCO-08 standards. Read more at: [International Standard Classification of Occupations (ISCO)](https://ilostat.ilo.org/methods/concepts-and-definitions/classification-occupation/)

- **Limitations**:  
  - Missing or incomplete data for some countries and years.
  - Vietnam analysis limited to 2010, 2012, 2014, and 2016 due to survey availability.
  - Wage bill fluctuations may reflect economic conditions as well as political events (e.g., crises, reforms).

---
