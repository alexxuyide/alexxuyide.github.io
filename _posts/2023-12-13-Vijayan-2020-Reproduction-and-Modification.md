---
title: "Vijayan Reproduction and Modification"
date: 2023-12-13
categories:
  - Reproduction Blog
tags:
  - Vijayan 2020
  - Reproducibility and Replicability
  - COVID-19
  - Los Angeles
  - Open Source GIScience
---

Vijayan et al. in the study “[Beyond the 405 and the 5: Geographic Variations and Factors Associated With Severe Acute Respiratory Syndrome Coronavirus 2 (SARS-CoV-2) Positivity Rates in Los Angeles County](https://doi.org/10.1093/cid/ciaa1692)” used geospatial modeling to examine the spatial pattern of response variables such as age-adjusted testing rates, age-adjusted diagnosis rates, and crude positivity rates in Los Angeles County (LAC), as well as how socio-structural characteristics are associated with these response variables. Building upon Kendron et al.’s reproduction of this study in 2020, Katie and I modified the reproduction study and improved its validity by fixing the connectivity issue of the hexagon grids used in the study and changing the misidentified variables. In addition, we constructed the metadata for this study, facilitating open access to both data and results for future reproductions on this study. 

We noticed several threats to the validity of the Vijayan study. The original data we received from the original study is the aggregated hexagon grid with census and COVID-19-related information. However, the original study does not indicate the assumptions and reasoning for translating the raw data (census data and COVID-19 data) from different units into the standardized 10-square-kilometer hexagon grids. The arbitrariness of this decision may affect the spatial relationship that we are modeling. Therefore, the study design is prone to scale distortion. Other distortions include boundary distortions. The authors associated the raw data with the hexagon grid by the centroid of the input data, ignoring the degree of geographic overlap between the hexagon grid and the source data as well as the diversity of size and shape of the raw data units. Additionally, because LA County is adjacent to the ocean, the density calculation of the hexagons near the ocean may not truly reflect the real density there. 

[Here is our html report of Vijayan Reproduction and Modification.](https://katieheo.github.io/Rpr-Vijayan-2023/)

[Here is the link to the repository](https://github.com/katieheo/Rpr-Vijayan-2023)

-------------
Bibliography:

Tara Vijayan, Michael Shin, Paul C Adamson, Christina Harris, Teresa Seeman, Keith C Norris, David Goodman-Meza, Beyond the 405 and the 5: Geographic Variations and Factors Associated With Severe Acute Respiratory Syndrome Coronavirus 2 (SARS-CoV-2) Positivity Rates in Los Angeles County, Clinical Infectious Diseases, Volume 73, Issue 9, 1 November 2021, Pages e2970–e2975, [https://doi.org/10.1093/cid/ciaa1692](https://doi.org/10.1093/cid/ciaa1692)