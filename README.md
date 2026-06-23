# Global Seismic Risk Profiles

<div align='center'>

<p align="center">
<img src="https://cloud-storage.globalquakemodel.org/public/Logos/GEM-LOGO-Red-RGB-300DPI.jpg" alt="GEM Foundation" width="300"/>
</p>

<a href='https://hazard.openquake.org/gem/'>
<img src='https://img.shields.io/badge/Global_Hazard_Model-green?style=for-the-badge'>
</a>

<a href='https://github.com/gem/global_vulnerability_model/'>
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

> The v2026.0.0 release for GEM's global seismic risk profiles is now available! 🥳 🚀

This repository hosts GEM's seismic risk profiles for 204 countries and territories worldwide. These seismic risk profiles have been produced with the outputs from the 2026 Global Seismic Risk Model of the GEM Foundation. Useful information about the underlying datasets and overall methodology can be found in the [Global Seismic Risk Model documentation](https://docs.openquake.org/global_risk_model/).


# 🚀 Profile versions  

Each version of the risk profiles that has been released can be accessed by changing from the `master` branch to the `tag` of a given version.

| Version   | Release Notes                                                            |
|-----------|--------------------------------------------------------------------------|
| [v2026.0.0](https://github.com/gem/risk-profiles/tree/v2026.0.0) | Release of the Global Risk Model (June 2026). This uses the exposure version `v2026.0.0`, vulnerability version `v2026.0.0`, and the relevant hazard model versions indicated per the global hazard map `v2026.1`. |
| [v2023.0.0](https://github.com/gem/risk-profiles/tree/v2023.0.0) | Release of the Global Risk Model (June 2023). This uses the exposure version `v2023.1.0`, vulnerability version `v2023.0.0`, and the relevant hazard model versions indicated per the global hazard map `v2023.1`. |
| v2018.0.0 | Original version within the larger 2018 Global Risk Model release.       |

# 🌍 Region and country list

<p align="center">
  <img src="./World/World_Regions.png" alt="World regions" width="600">
</p>

The following countries/territories are covered in this repository, organized by risk regions as indicated in the table below. 

| REGION                    | COUNTRIES & TERRITORIES |
|---------------------------|-----------|
| **Africa** | Algeria, Angola, Benin, Botswana, Burundi, Cabo Verde, Cameroon, Central African Republic, Comoros, Congo, Democratic Republic of the Congo, Djibouti, Egypt, Equatorial Guinea, Eritrea, Eswatini, Ethiopia, Gabon, Gambia, Ghana, Guinea, Guinea Bissau, Ivory Coast, Kenya, Lesotho, Liberia, Libya, Madagascar, Malawi, Mali, Mauritania, Mauritius, Morocco, Mozambique, Namibia, Nigeria, Rwanda, Senegal, Sierra Leone, Somalia, South Africa, South Sudan, Sudan, Tanzania, Togo, Tunisia, Uganda, Zambia, Zimbabwe |
| **Caribbean Central America** | Anguilla, Antigua and Barbuda, Aruba, Bahamas, Barbados, Belize, British Virgin Islands, Cayman Islands, Costa Rica, Cuba, Dominica, Dominican Republic, El Salvador, Grenada, Guadeloupe, Guatemala, Haiti, Honduras, Jamaica, Martinique, Montserrat, Nicaragua, Panama, Puerto Rico, Saint Kitts and Nevis, Saint Lucia, Saint Vincent and the Grenadines, Trinidad and Tobago, Turks and Caicos Islands, US Virgin Islands |
| **Central Asia** | Kazakhstan, Kyrgyzstan, Tajikistan, Turkmenistan, Uzbekistan |
| **East Asia** | Mainland China, Hong Kong, Japan, Macao, North Korea, South Korea, Taiwan |
| **Europe** | Albania, Andorra, Austria, Belarus, Belgium, Bosnia and Herzegovina, Bulgaria, Croatia, Cyprus, Czechia, Denmark, Estonia, Finland, France, Germany, Gibraltar, Greece, Hungary, Iceland, Ireland, Isle of Man, Italy, Kosovo, Latvia, Liechtenstein, Lithuania, Luxembourg, Malta, Moldova, Monaco, Montenegro, Netherlands, North Macedonia, Norway, Poland, Portugal, Romania, Serbia, Slovakia, Slovenia, Spain, Sweden, Switzerland, Turkiye, Ukraine, United Kingdom |
| **Middle East** | Armenia, Azerbaijan, Bahrain, Georgia, Iran, Iraq, Israel, Jordan, Kuwait, Lebanon, Oman, Palestine, Qatar, Saudi Arabia, Syria, United Arab Emirates, Yemen |
| **North America** | Canada, Mexico, United States |
| **North Asia** | Mongolia, Russia |
| **Oceania** | American Samoa, Australia, Fiji, Guam, Micronesia, New Caledonia, New Zealand, Niue, Northern Mariana Islands, Palau, Papua New Guinea, Samoa, Solomon Islands, Tonga, Vanuatu |
| **South America** | Argentina, Bolivia, Brazil, Chile, Colombia, Ecuador, French Guiana, Guyana, Paraguay, Peru, Uruguay, Venezuela |
| **South Asia** | Afghanistan, Bangladesh, Bhutan, India, Nepal, Pakistan, Sri Lanka |
| **Southeast Asia** | Brunei, Cambodia, Indonesia, Laos, Malaysia, Myanmar, Philippines, Singapore, Thailand, Timor Leste, Vietnam |

# 📋 Explanation of profile content

The GEM Foundation has produced a collection of Country/Territory Seismic Risk Profiles that summarize key metrics of seismic risk, allowing stakeholders in risk management to get an overview of the risk in a region at-a-glance. Each profile presents the following relevant information:

* Social indicators, which provide context to the region in question 
* Risk indicators, detailing an occupancy breakdown of exposed value and losses
* A list of the major earthquakes that have impacted the region
* Loss per region, providing a breakdown of average annual losses per administrative level 1
* Building classes, depicting the major construction materials used in the region
* Loss curves, which provide expected losses per different return periods
* Maps depicting the geographical distribution of hazard, exposure, and losses

The risk values presented are the results of an event-based risk analysis, where 100,000 years of earthquakes are simulated. Three lines of business are considered: residential, commercial, and industrial. Therefore, the value or earthquake losses from damage to other building occupancies (e.g., schools, healthcare) and infrastructure are not included.

# 👨‍👩‍👧‍👦 Related datasets and resources

Users interested in these seismic risk profiles might also find the following GEM products useful:

* [Global Seismic Risk Map](https://www.globalquakemodel.org/products/global-seismic-risk-map)
* [Global Seismic Hazard Map](https://www.globalquakemodel.org/product/global-seismic-hazard-map)
* [Global Exposure Model](https://www.globalquakemodel.org/product/global-exposure-model)
* [Global Vulnerability Model](https://www.globalquakemodel.org/product/global-vulnerability-model)
* [OpenQuake engine](https://www.globalquakemodel.org/product/openquake-engine)

# 📚 Publications

Please cite the work as follows:

A. Rao, K. Aljawhari, M. Baiguera, A. Calderón, M. Caruso, C. Costa, D. González, A. M. B Nafeh, M. Nastasi, M. Simionato, V. Silva, C. Yepes-Estrada (2026), Country/Territory Seismic Risk Profiles of the GEM Foundation. https://github.com/gem/risk-profiles/

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8431824.svg)](https://doi.org/10.5281/zenodo.8431824)


# 🌟 Contributors 

The authors are grateful for the input from dozens of local and international experts. A list of contributors can be found at https://www.globalquakemodel.org/risk-model-contributors.


# 📃 License
[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa], which requires:

* Attribution (you must give appropriate credit, provide a link to the license, and indicate if changes were made)
* Non-commercial (you may not use the material for commercial purposes)
* ShareAlike (derivatives created must be made available under the same license as the original)

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

Any deviation from these terms incur in license infringement. For commercial use of the data contained within this work, a specific license agreement must be made tailored to your use case, in such instance please contact GEM at product@globalquakemodel.org


# 🤔 Frequently asked questions 

### Where can I find documentation related to this product?
Useful information about the underlying datasets and overall methodology can be found in the [Global Seismic Risk Model documentation](https://docs.openquake.org/global_risk_model/).

### Which version am I seeing? How to change the version?
By default you will see the files in the repository in the  `master` branch. Each version of the model that is released can be accessed is marked with a `tag`. By changing the tag version at the top of the repository, you can change see the files for a given version.

Note that the `master` branch could contain the work-in-progress of the next version of the model.

### How do I download the data for a given version?
For each version, a related zip file is available in the [release section](https://github.com/gem/risk-profiles/releases).

### Where can I find the models at the highest available resolution?

Please contact us at product@globalquakemodel.org

### What if my use case does not comply with the Creative Commons license offered?

If your use case deviates from the requirements of the offered license, but still want to explore the use of the data, please contact us at license@globalquakemodel.org 
