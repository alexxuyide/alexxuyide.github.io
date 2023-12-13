---
title: "Spielman 2020 Reproduction and Modification"
date: 2023-11-01
categories:
  - Reproduction Blog
tags:
  - Spielman 2020
  - Reproducibility and Replicability
  - Social Vulnerability Index
  - Open Source GIScience
---


We have successfully reproduced [Spielman’s study](https://doi.org/10.1007/s11069-019-03820-z) of the Social Vulnerability Index (SoVI), based on the method developed by [Cutter et al.](https://doi.org/10.1111/1540-6237.8402002), across all counties in the United States. We calculated SoVI in three scales (nationally, by FEMA region, and by sample states) and got the same results in all of them in our reproduction study. To improve the theoretical consistency, we further explore the social vulnerability index calculation by introducing the percentage of variance in SoVI explained by each component of the model to give us the final social vulnerability index. We were surprised to find that the ranking of the weighted SoVI is almost similar to the ranking of the unweighted SoVI in the original study. The result from the weighted calculation of SoVI suggests that further investigation into the method’s accuracy may be warranted.

The revised reproduction study also added a visualization of the national scale SoVI score distribution, the national scale difference between weighted SoVI and unweighted SoVI, and a table in the Principal Component Analysis section presenting how much weight is assigned to each variable of each principal component. 

[Here is my html report of Spielman Reproduction and Modification.](https://alexxuyide.github.io/RPl-Spielman-2020/)

[Here is the link to the repository](https://github.com/alexxuyide/RPl-Spielman-2020)


-------------
Bibliography:

Cutter, S. L., Boruff, B. J., & Shirley, W. L. (2003). Social vulnerability to environmental hazards. Social Science Quarterly, 84(2), 242–261. [https://doi.org/10.1111/1540-6237.8402002](https://doi.org/10.1111/1540-6237.8402002)

Spielman, S. E., Tuccillo, J., Folch, D. C., Schweikert, A., Davies, R., Wood, N., & Tate, E. (2020). Evaluating social vulnerability indicators: criteria and their application to the Social Vulnerability Index. Natural Hazards, 100(1), 417–436. [https://doi.org/10.1007/s11069-019-03820-z](https://doi.org/10.1007/s11069-019-03820-z)