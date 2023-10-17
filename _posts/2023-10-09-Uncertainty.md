---
title: "Provenance, Error and Uncertainty"
categories:
  - General Blog
tags:
  - Uncertainty
  - Open Source GIScience
  - Discussion
---

The research project I conducted this summer when I used SAM to quantify the smallholder woodlots is an example of my experience with uncertainty. We were trying to test the accuracy of our developed method in detecting the right woodlots, and we encountered uncertainties in the representation and analysis step. Due to the dynamic nature of the landscape, the ground truth data of smallholder woodlots are not applicable now. We have to select the current-day woodlots for referencing from the outdated ground truth data. The only reference we could use to detect woodlots was the satellite image, and we were not 100% confident that the land features we identified were actually woodlots. This could produce errors in measurement. During the analysis process, the SAM’s performance in a heterogeneous landscape further added uncertainty. Given the image scale, it was not able to segment all the land features from the landscapes (for example, SAM cannot identify individual trees of a new woodlot). In addition, our preliminary method of using linear regression of the Tasselled Cap Wetness index to determine which segments were smallholder woodlots is oversimplified. At last, we have a considerable amount of omission errors. The uncertainty added in each step of the analysis contributes to the final accuracy. 

Reading the article by Longley et. al. (2008), I believe one of the most important responsibilities that geographers have is to acknowledge the existence of uncertainties in each step of their research. It is impossible to circumvent uncertainties when conducting research, but geographers should try to minimize it. I think there are several strategies that geographers should implement to fullfil the responsibility of recognizing and live with uncertainty. The first step is formalizing the language when describing the phenomena in order to avoid logical fallacy and communication errors. The second step is to develop a categorizing list of uncertainties, exhausting all possible methods that geographers use. Ideally, it would be beneficial to identify which type of uncertainties could be most harmful to research and develop a metric to quantify the errors. The third strategy is to reinforce supervision, which could be peer check and reproduction studies. The review process is a collaborative effort to identify and minimize the occurrence of uncertainty. 
