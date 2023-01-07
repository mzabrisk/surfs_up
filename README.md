# surfs_up

## Overview
We are considering opening up a surf shop in Oahu, but more details regarding the temperature in both winter and summer are needed to determine if it can be a successful year-round business. Specifically, we have been asked to look at the temperatures in June and December.


## Results
This query was used to return the June temperatures:
![](https://github.com/mzabrisk/surfs_up/blob/81193529495a17cca3e93b8c4681ec999989fe41/figures/june_temps_query.png)

This query was used to return the December temperatures:
![](https://github.com/mzabrisk/surfs_up/blob/81193529495a17cca3e93b8c4681ec999989fe41/figures/december_temps_query.png)

And the resulting summary statistics were produced:
![](https://github.com/mzabrisk/surfs_up/blob/81193529495a17cca3e93b8c4681ec999989fe41/figures/june_temps_summary_stats.png)
![](https://github.com/mzabrisk/surfs_up/blob/81193529495a17cca3e93b8c4681ec999989fe41/figures/december_temps_summary_stats.png)

Overall, the weather between June and December is surprisingly similar, however there are a few key differences.

The 3 main take aways from these results are:
- The median temperature in June is 75F, while the median temperature in December is 71F. While June is a little warmer, the temperatures are usually comfortable both months. Additionally, the mean temperature for both months is very similar to the median (74.9F in June and 71F in December), indicating that the distribution is likely normal.

- The temperature in June ranges from a high of 85F to a low of 64F (range of 21F). The temperature in December ranges from 83F to 56F (range of 27F). Looking at these numbers alone indicates there could be drastic swings in weather during a given month.

- However, in June the 1st quartile is 73F, and the 3rd quartile is 77F. In December the 1st quartile is 69F, and the 3rd quartile is 74F. This gives us an IQR of 4F and 5F for June and December, respectively. Such a small IQR indicates that there is usually little variation in the temperatures, so the high and/or low temperatures are possibly outliers. For this analysis, a histogram or box and whisker plot could be a useful addition.


## Summary
Overall, the weather in both June and December looks remarkably similar, and both would be great times of year to go surfing in Oahu. From the current dataset, it would also be worth looking at the precipitation data. A sample query doing so using the June data is present here:
![](https://github.com/mzabrisk/surfs_up/blob/c187834645bff3345dce898e1ad6427d5ada9122/figures/june_prcp_query_stats.png)

It would also be useful to include histograms of the data (both temperatures and precipitation) to make it easier to see how the weather is distributed. This analysis should also be conducted for all months - it may be the case that a different month is extremely rainy or cool and less ideal for surfing. Although not included in the README.md summary, these histograms were generated in the SurfsUp_Challenge.ipynb file.

A different dataset would need to be obtained, but an analysis of the water conditions - including wave size and water temperatures - would likely be even more useful than weather data. However, a different dataset would be required for this.