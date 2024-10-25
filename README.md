# With Africa Platform

Welcome to the **With Africa** platform repository! This project is dedicated to facilitating data-driven insights and analysis for sustainable tourism across Africa. Here, you'll find resources, including datasets, analysis notebooks, and scripts, that contribute to our mission of enhancing tourism understanding and decision-making across the continent.

## Overview
The **With Africa Tourism Data Platform** repository houses Jupyter notebooks, data processing scripts, and data files, supporting researchers, policymakers, and developers interested in the African tourism landscape. The focus is on providing clean, structured datasets and reproducible code to advance sustainable and data-driven tourism.

## Table of Contents
- [With Africa Platform](#with-africa-platform)
  - [Overview](#overview)
  - [Table of Contents](#table-of-contents)
  - [Folder Structure](#folder-structure)
  - [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
    - [Usage](#usage)
      - [Datasets](#datasets)
      - [Data Processing](#data-processing)
      - [Data Analysis](#data-analysis)
  - [License](#license)

## Folder Structure
```
with-africa-tourism-data-platform/
├── datasets/                  # Contains all datasets used for analysis and dashboards
│   ├── ade/                   # African Tourism Data Ecosystem related datasets
│   │   ├── open_data_sources.xlsx
│   │   └── results.xlsx
│   ├── dashboards/            # Data used for country profiles dashboards
│   ├── ddt/                   # Data related to the Data Discovery Tool
│   │   └── ddt_complete.xlsx
│   ├── general/               # General tourism and related datasets
│   │   ├── CPI2023_Global_Results__Trends.xlsx
│   │   ├── conf_venues_afr.pdf
│   │   ├── Mapping Academia (new).xlsx
│   │   └── other files
│   ├── new_platform/          # Datasets for the new platform setup
│   │   └── about_our_data/
│   │       ├── about_data.xlsx
│   ├── country_profiles/      # Data used for creating country profiles
│   │   ├── country_cultural.xlsx
│   │   ├── country_profiles.xlsx
│   │   └── un_sites_2024.xlsx
│   ├── research/              # Datasets used in research analysis
│   │   ├── iata_afr_airlines.xlsx
│   └── unwto/                 # UNWTO datasets
│       ├── unwto-all-data-download_032023.xlsx
│       ├── unwto-all-data-download_112023.xlsx
│       └── countryContUNWTO.xlsx
└── notebooks/                 # Contains Jupyter notebooks for data processing and analysis
    ├── about_our_data/
    │   └── similarity-algo.ipynb   # Obtains similar indicators for the data page
    ├── ade/
    │   └── analysis.ipynb          # Analysis for the African Tourism Data Ecosystem dashboard
    ├── composite_indicators/
    │   ├── business_indicatorss.ipynb    # Creates business indicator using factor analysis
    │   └── sunburst_plot.html            # Visualization for business indicators
    ├── country_profiles/
    │   ├── get_wb_data_country_profiles.ipynb   # Obtains World Bank data for country profiles
    │   └── wikidata_country_profiles.ipynb      # Processes country profile data from Wikidata
    ├── data_discovery_tool/
    │   ├── ddt_database.ipynb      # Cleans and processes the latest UNWTO Excel file
    │   └── get_worldbank_data.ipynb # Obtains and processes World Bank tourism data
    ├── dataset_setup/
    │   └── platform_setup.ipynb    # Sets up platform with new datasets and analysis pipelines
    ├── research/
    │   └── business_report/
    │       ├── business_analysis.ipynb   # Data processing and analysis for business report
    │       └── visastat.png              # Visualization for business report analysis
    └── rising_tides/
        └── clustering_industry_demo.ipynb  # Clustering countries based on tourism performance
```


## Getting Started

### Prerequisites
- **Python 3.12+**
- [Jupyter Notebook](https://jupyter.org/install)
- Recommended Python packages (see `requirements.txt`)

### Installation
1. **Clone the repository**:
   ```bash
   git clone [LINK]
   ```
2. **Navigate to the project directory**:
   ```bash
   cd with-africa-platform
   ```
3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
### Usage
#### Datasets

> The repository contains several key datasets used for analysis and dashboarding purposes. These datasets are divided into multiple folders:

`ade/`

- open_data_sources.xlsx: Contains data sources used for the African Tourism Data Ecosystem (ADE) dashboard.
- results.xlsx: Results of the ADE analysis.

`ddt/`

- ddt_complete.xlsx: Complete dataset related to the data discovery tool and other related processing.

`dashboards/`

- This folder contains the data used for the country profiles dashboard, including indicators and various metrics relevant for African tourism.

`general/`

- conf_venues_afr.pdf: Information on African conference venues.
- CPI2023_Global_Results__Trends.xlsx: Global results for the 2023 CPI.
- data_discovery_db.sqlite: SQLite database for data discovery and processing.
- Mapping Academia (new).xlsx: Academic mapping for tourism-related research.
- global_peace_index_2024.xlsx: Data related to global peace indices for 2024.
- num_conference_venues.xlsx: Dataset on the number of conference venues.
- ookla_speed_test.xlsx: Internet speed test results from Ookla.
- WEF_TTDI_2021_data_for_download.xlsx: WEF TTDI data for 2021.
- WEF_TTDI_2024_edition_data.xlsx: WEF TTDI 2024 edition data.
- whc-sites-2023.xls: UNESCO world heritage sites for 2023.
- whc-sites-2024.xls: UNESCO world heritage sites for 2024.

`new_platform/about_our_data/`

- about_data.xlsx: Data used for explaining indicators and metrics on the ‘About Our Data’ page.

`country_profiles/`

- country_cultural.xlsx: Cultural data relevant for the country profiles dashboard.
- country_profiles.xlsx: Core data related to African country profiles.
- un_sites_2024.xlsx: Data on United Nations sites relevant to the country profiles.

`ddt_comp_with_sim.xlsx`

- Dataset containing comparisons with similarity analysis relevant to the data discovery tool.

`eoa/results.xlsx`

- Results dataset used in the analysis for the End of Africa report.

research/business_report/`

- iata_afr_airlines.xlsx: Data on IATA African airlines for business report analysis.

`unwto/`

- countryContUNWTO.xlsx: Country-level data for UNWTO statistics.
- unwto-all-data-download_032023.xlsx: UNWTO tourism data for March 2023.
- unwto-all-data-download_112023.xlsx: UNWTO tourism data for November 2023.

`world_bank/`

- WDIEXCEL.xlsx: World Bank World Development Indicators.
- world_bank_indicators.xlsx: Additional tourism-relevant indicators from the World Bank.

#### Data Processing

- Data Discovery Tool: In the data_discovery_tool/ directory, there are scripts for processing and cleaning tourism data:
- ddt_database.ipynb: Cleans and processes the latest UNWTO Excel file with 145 tourism indicators.
- get_worldbank_data.ipynb: Obtains and processes tourism data from the World Bank.
- Country Profiles: The country_profiles/ directory contains notebooks to obtain data relevant for country profile dashboards:
- get_wb_data_country_profiles.ipynb: Fetches World Bank data for country profiles.
- wikidata_country_profiles.ipynb: Processes country profile data from Wikidata.
- Similarity Algorithm: The about_our_data/similarity-algo.ipynb notebook is used to identify similar indicators for the data page.

#### Data Analysis

- ADE: The ade/analysis.ipynb notebook contains analysis related to the African Tourism Data Ecosystem dashboard.
- Business Indicators: In the composite_indicators/ folder, the business_indicatorss.ipynb notebook builds a business indicator using factor analysis, while the sunburst_plot.html provides a visualization.
- Business Report: The research/business_report/ directory contains the business_analysis.ipynb notebook for business report data processing and analysis, including the visastat.png visualization.
- Rising Tides: The rising_tides/clustering_industry_demo.ipynb notebook demonstrates the clustering algorithm used to group countries based on tourism performance.
## License
 <p xmlns:cc="http://creativecommons.org/ns#" >This work is licensed under <a href="https://creativecommons.org/licenses/by-nc/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY-NC 4.0<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1" alt=""><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1" alt=""><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/nc.svg?ref=chooser-v1" alt=""></a></p> 

