---
title: "Kang 2020 Reproduction and Modification"
date: 2023-11-01
categories:
  - Reproduction Blog
tags:
  - Kang 2020
  - Reproducibility and Replicability
  - Healthcare Resource Accessibility
  - COVID-19
  - Chicago
  - Open Source GIScience
---

Kang et al.’s study focuses on mapping and analyzing the accessibility of COVID-19 healthcare resources in Chicago and the state of Illinois using network analysis. In our reproduction and reanalysis project, we reproduced the study’s analysis in the Chicago area where we followed the original study by 1) producing hospitals’ service areas (10, 20, and 30-minute driving distance); 2) calculating the service-to-population ratio, and 3) aggregating the accessibility score in the Chicago hexagon grid. We later proposed alternative approaches to the study’s methodology components of Step 1) and Step 3), which are improving the network’s speed limit data and introducing the area-weighted reaggregation method to the score calculation step. 

We used OSMNX packages to fix the road segments without speed limits. Instead of assigning 35 mph to all the segments that do not have a speed limit, the OSMNX package fills the void by assigning the average speed limit of the same road-type segments with speed limit data. This method ensures that the analysis is based on data that is more realistic and could better simulate the result. When calculating the accessibility score, the original study employs an “all-or-nothing” approach which assigns the rate of a given catchment area to the entire hexagon if more than 50 percent of the hexagon is covered by the catchment area. By using the area-weighted reaggregation method in accessibility score calculation, we could improve the precision by taking into account the hexagons that are covered less than 50 percent by the hospital catchment area. 

[Here is my html report of Kang Reproduction and Modification.](https://alexxuyide.github.io/RPl-Spielman-2020/)

[Here is the link to the repository](https://github.com/alexxuyide/RPr-Kang-2020)



-------------
Bibliography:

Kang, J. Y., A. Michels, F. Lyu, Shaohua Wang, N. Agbodo, V. L. Freeman, and Shaowen Wang. 2020. Rapidly measuring spatial accessibility of COVID-19 healthcare resources: a case study of Illinois, USA. International Journal of Health Geographics 19 (1):1–17. DOI:[10.1186/s12942-020-00229-x](https://doi.org/10.1186/s12942-020-00229-x).
