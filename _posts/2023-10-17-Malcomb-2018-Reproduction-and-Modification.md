---
title: "Malcomb 2018 Reproduction and Modification"
date: 2023-10-17
categories:
  - Reproduction Blog
tags:
  - Malcomb 2021
  - Reproducibility and Replicability
  - Vulnerability
  - Open Source GIScience
---

The second reproduction and modification study we implemented is ["Vulnerability modeling for sub-Saharan Africa: An operationalized approach in Malawi"](https://www.sciencedirect.com/science/article/abs/pii/S0143622814000058?via%3Dihub) by Dylan W. Malcomb. Here are my plans to modify and contribute to the study. 

- Plan 1:

There is little documentation about how different data is calculated to get the adaptive capacity and vulnerability score in the original study. Therefore, in the reproduction study, the first group of contributors figured the process by themselves about how the score should be calculated. There are some inconsistency about discrete or continuous data in the reproduction study. I am going to identify where are these discrepancies of data and try to make most of them continuous in order to presever the best accuracy. 

- Plan 2:

The vulnerability score is calculated on raster scale, but the adaptive capacity is calculated in traditional authority boundaries (TA) and the livelihood data is in livelihood region scale. There is a confusion of scale on how the data is recorded, analyzed, and presented. To preserve the consistency of data representation, I will try to present the map of vulnerability score in a TA scale, just like how adaptive capacity is presented. 

- Plan 3: 

I am going to write a discussion and conclusion part of this reproduction study to make it complete. 