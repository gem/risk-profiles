# Global Risk Profiles

<div align='center'>

<p align="center">
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5b/Global_Earthquake_Model_Logo.png/440px-Global_Earthquake_Model_Logo.png" alt="GEM Foundation" width="300"/>
</p>

<a href='https://hazard.openquake.org/gem/'>
<img src='https://img.shields.io/badge/Global_Hazard_Model-green?style=for-the-badge'>
</a>

<a href='https://docs.openquake.org/vulnerability/'>
<img src='https://img.shields.io/badge/Global_Vulnerability_Model-gray?style=for-the-badge'>
</a>

<a href='https://github.com/gem/global_exposure_model'>
<img src='https://img.shields.io/badge/Global_Exposure_Model-orange?style=for-the-badge'>
</a>

<a href='LICENSE.txt'>
<img src='https://img.shields.io/badge/LICENSE-blue?style=for-the-badge'>
</a>

</div>

# ✨ Overview

> The v2023.0.0 release for the GEM's global earthquake risk profiles is now available! 🥳 🚀

This repository hosts the global earthquake risk profiles for the world.


# 🚀 Model versions  

Each version of the model that is released can be accessed by changing from the `master` branch to the `tag` of a given version.
The `master` branch could contain the work-in-progress of the next version of the model.

| Version   | Release Notes                                                            |
|-----------|--------------------------------------------------------------------------|
| v2018.0.0 | Original version within the larger 2018 Global Risk Model release.       |
| [v2023.0.0](https://github.com/gem/risk-profiles/tree/v2023.0.0) | Release of the Global Risk Model (June 2023). |

# 🌍 Region and country list

<p align="center">
  <img src="./World/World_Regions.png" alt="World regions" width="600">
</p>

The following countries/territories are covered in this repository, organized by risk regions as indicated in the table below. 

| REGION                    | COUNTRIES & TERRITORIES |
|---------------------------|-----------|
| Africa                    | Algeria, Angola, Benin, Botswana, Burkina_Faso, Burundi, Cameroon, Cape_Verde, Central_African_Republic, Chad, Comoros, Congo, Democratic_Republic_of_the_Congo, Djibouti, Egypt, Equatorial_Guinea, Eritrea, Eswatini, Ethiopia, Gabon, Gambia, Ghana, Guinea, Guinea_Bissau, Ivory_Coast, Kenya, Lesotho, Liberia, Libya, Madagascar, Malawi, Mali, Mauritania, Mauritius, Morocco, Mozambique, Namibia, Niger, Nigeria, Rwanda, Sao_Tome_and_Principe, Senegal, Seychelles, Sierra_Leone, Somalia, South_Africa, South_Sudan, Sudan, Tanzania, Togo, Tunisia, Uganda, Zambia, Zimbabwe |
| Caribbean_Central_America | Anguilla, Antigua_and_Barbuda, Aruba, Bahamas, Barbados, Belize, British_Virgin_Islands, Cayman_Islands, Costa_Rica, Cuba, Dominica, Dominican_Republic, El_Salvador, Grenada, Guadeloupe, Guatemala, Haiti, Honduras, Jamaica, Martinique, Montserrat, Nicaragua, Panama, Puerto_Rico, Saint_Kitts_and_Nevis, Saint_Lucia, Saint_Vincent_and_the_Grenadines, Trinidad_and_Tobago, Turks_and_Caicos_Islands, US_Virgin_Islands |
| Central_Asia              | Kazakhstan, Kyrgyzstan, Tajikistan, Turkmenistan, Uzbekistan |
| East_Asia                 | China, Hong_Kong, Japan, Macao, North_Korea, South_Korea, Taiwan |
| Europe                    | Albania, Andorra, Austria, Belarus, Belgium, Bosnia_and_Herzegovina, Bulgaria, Croatia, Cyprus, Czechia, Denmark, Estonia, Finland, France, Germany, Gibraltar, Greece, Hungary, Iceland, Ireland, Isle_of_Man, Italy, Kosovo, Latvia, Liechtenstein, Lithuania, Luxembourg, Malta, Moldova, Monaco, Montenegro, Netherlands, North_Macedonia, Norway, Poland, Portugal, Romania, Serbia, Slovakia, Slovenia, Spain, Sweden, Switzerland, Turkey, Ukraine, United_Kingdom |
| Middle_East               | Afghanistan, Armenia, Azerbaijan, Bahrain, Georgia, Iran, Iraq, Israel, Jordan, Kuwait, Lebanon, Oman, Pakistan, Palestine, Qatar, Saudi_Arabia, Syria, United_Arab_Emirates, Yemen |
| North_America             | Canada, Mexico, United_States_of_America |
| North_Asia                | Mongolia, Russia |
| Oceania                   | American_Samoa, Australia, Cook_Islands, Fiji, Guam, Kiribati, Marshall_Islands, Micronesia, Nauru, New_Caledonia, New_Zealand, Niue, Northern_Mariana_Islands, Palau, Papua_New_Guinea, Samoa, Solomon_Islands, Tonga, Tuvalu, Vanuatu |
| South_America             | Argentina, Bolivia, Brazil, Chile, Colombia, Ecuador, French_Guiana, Guyana, Paraguay, Peru, Suriname, Uruguay, Venezuela |
| South_Asia                | Afghanistan, Bangladesh, Bhutan, India, Nepal, Pakistan, Sri_Lanka |
| Southeast_Asia            | Brunei, Cambodia, Indonesia, Laos, Malaysia, Myanmar, Philippines, Singapore, Thailand, Timor_Leste, Vietnam |

# Explanation of exposure model content

## Definition of column headers

Each exposure csv contains the following column headers, as briefly defined below

- **ASSET_ID**: Unique identifier for an asset, which comprises a group of buildings sharing similar attributes and location
- **ID_1**: ID for the first administrative level, matches either the ID used in the national census or in the administrative division boundary vector files, or both
- **NAME_1**: Name of the first administrative level
- **ID_2**: ID for the second administrative level
- **NAME_2**: Name of the second administrative level
- ⋮
- **LONGITUDE**, **LATITUDE**: Geographical coordinates assigned to the asset for risk calculations. In general, these locations do not represent building-specific geolocations, but are either aggregated at a representative point for the lowest administrative level or are the result of the spatial disaggregation algorithm (and thus still represent aggregated assets, but at a finer resolution)
- **OCCUPANCY**: The primary occupancy class: Res for residential, Com for commercial, and Ind for industrial
- **TAXONOMY**: Building taxonomy string that is used for mapping vulnerability functions for the asset
- **BUILDINGS**: The total number of buildings comprising the asset
- **TOTAL_AREA_SQM**: The total floor area comprising the asset (sq.m.)
- **COST_PER_AREA_USD**: The average replacement cost per unit area (in 2021 US$/sq.m., including the structural and nonstructural components, but not the building contents) 
- **TOTAL_REPL_COST_USD**: The total replacement cost for the asset (in 2021 US$, including the structural, nonstructural components, and building contents) 
- **COST_STRUCTURAL_USD**: The cost of structural components in each asset
- **COST_NONSTRUCTURAL_USD**: The cost of nonstructural components in each asset
- **COST_CONTENTS_USD**: The cost of contents in each asset
- **OCCUPANTS_PER_ASSET**: The number of residents in each residential asset
- **OCCUPANTS_PER_ASSET_DAY**: The average number of occupants in each asset (residential, commercial, industrial) during the day time period
- **OCCUPANTS_PER_ASSET_TRANSIT**: The average number of occupants in each asset (residential, commercial, industrial) during the transit time period
- **OCCUPANTS_PER_ASSET_NIGHT**: The average number of occupants in each asset (residential, commercial, industrial) during the night time period
- **OCCUPANTS_PER_ASSET_AVERAGE**: The time-averaged number of occupants in each asset (residential, commercial, industrial) 

## Where can I find additional information on the defined building classes?

The building classes defined within this exposure model follow the GEM Taxonomy convention. Please refer to the [GEM Taxonomy Glossary](https://taxonomy.openquake.org/) for additional details on taxonomy substrings.


# 📚 Publications

Please cite the work as follows:
TODO

TODO: Repository DOI (Zenodo)


# 🌟 Contributors 

The authors are grateful for the input from dozens of local and international experts. A list of contributors can be found at https://www.globalquakemodel.org/risk-model-contributors.


# License
[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg


# 🤔 Frequently asked questions 

### Which version am I seeing? How to change the version?
By default you will see the files in the repository in the  `main` branch. Each version of the model that is released can be accessed is marked with a `tag`. By changing the tag version at the top of the repository, you can change see the files for a given version.

Note that the `main` branch could contain the work-in-progress of the next version of the model.

### How do I download the data for a given version?
For each version, a related zip file is available in the [release section](https://github.com/gem/risk-profiles/releases).

### Where can I find the models at the highest available resolution?

Please contact us at product@globalquakemodel.org