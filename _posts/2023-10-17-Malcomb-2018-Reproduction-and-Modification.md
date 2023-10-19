---
title: "Malcomb 2018 Reproduction and Modification"
date: 2023-10-17
categories:
  - Reproduction Blog
tags:
  - Malcomb 2014
  - Reproducibility and Replicability
  - Vulnerability
  - Open Source GIScience
---

The second reproduction and modification study we implemented is ["Vulnerability modeling for sub-Saharan Africa: An operationalized approach in Malawi"](https://www.sciencedirect.com/science/article/abs/pii/S0143622814000058?via%3Dihub) by Dylan W. Malcomb. The study aimed to combine household and physical data of Malawi and develop a methodology to calculate country-scale vulnerability score for climate change. The reproduction of the study is not ideal, as there are large and random differences between the reproduction result and the original study. In my modfication plan, I plan to 
1. Identify discrepancy of discrete and continuous data.
2. Map vulernability score in Traditional Authority unit (raster to vector).
3. Write discussion section to explain the failure of reproduction. 

To meet **Plan 1**, I tried to preserve the continuity of drought data, which is a component of the physical exposure category, by rescaling the data to [0, 20] and apply it to the final vulnerability score. Compared with the vulnerability score map that used discrete drought data, the contribution of the continuous drought data on the final map is little. I suspect that there exists outlier data in drought data. For **Plan 2**, more than creating the vulnerability score in TA unit map for the reproduction data, I created a similar map for the original data and a comparison map between them. The TA unit vulnerability score map could be used to evaluate which regions have relatively higher vulnerability, and therefore more resource could be allocated or actions could take place these regions. The TA level vulnerability score comparison scale also helps us to find deviation introduced since the adaptive capacity step. The last step of my modification is to write a discussion section at the end of the study, which is my **Plan 3**. I identified three main reasons that could attribute to the faliure of reproduction: lacking important data and methodology in the original study, mixing continuous and discrete numerical data, and mixing vector and raster spatial data. 

[Here is my html report of Malcomb Reproduction and Modification.]()

[Here is the link to the repository](https://github.com/alexxuyide/RPr-Malcomb-2014)