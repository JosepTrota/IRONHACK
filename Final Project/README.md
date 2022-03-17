# CLUSTERING COUNTRIES :earth_africa:
## WHAT IS A NEIGHBORING COUNTRY IN THIS MODERN GLOBALIZATION ERA

***

What are neighboring countries? The answer seems obvious at first: countries sharing a frontera. But frontiers have been slowly getting more complex and even non material. First sea travel, then air travel, then space and the world wide web...

But we can try to discover which countries share some traits, in terms of subjective experiences.

What if a neighborhood of them is just a cluster of countries in which the experience of living is more or less the same, or at least kind of similar?

***

Since the mid 90s, a couple of political scientist, the american Ronald Inglehart and the german Christian Welzel, tried to organize clusters of countries around two different axis comprehending some country values: one mesuring the ratio of traditional vs secular values, and the other mesuring the ratio of survival vs self expression values.

Their current actualized map (from 2020) is this one:

![alt text](https://github.com/JosepTrota/IRONHACK/blob/main/Final%20Project/Inglehart%20-%20Welzel%20cultural%20map.jpg "You discovered the title remainder text. Hooray! You can have a cookie ;)")

As you can see, there are some criticism to be made:
* The axis consist of somewhat loose features
* There are clear outliers on the clusters
* There is no cluster consistency - they are sometimes geographic, sometimes religious, in anterior designs sometimes political...
* Could be ethnocentric or maybe even racist, implying that the countries at the top right have the *correct* values, and the bottom left have the least desirable ones (note that Inglehart is american and Welzel from the western part of Germany, both white males, with high academic profiles, so some bias could be there)

**How can we try to reduce bias and improve the creation of "neighbor countries"?**


***

## The idea

***

To show the most objective clusters possible, but taking into account some subjective data, we can look up some international indexes. We decided to focus on those pairs of index - source:

* IW cultural axis: world values survey
*	unpeacefulness: Institute for Economics and Peace
*	eco_footprint: Global Footprint Network
*	education: UNESCO
*	nominal_GDP: International Monetary Fund
*	inequality: CIA World Factbook - 2021
*	life_expectancy: the world bank
*	religion (all): CIA World Factbook - 2021
*	happiness: world happiness report


***

## The method

***

After lots and lots of exploratory data analysis and cleaning, we decided to use the KMeans clustering method, trying to use elbow method and silhouette score to validate the number of clusters in each case. We must say that the elbow method rarely gave us relevant information, and we used the silhouette score to decide which was the best number to pick.


***

## The results

***



***

## Later observations and conclusions

***



#### SWOT ABOUT THE PROJECT

Strengths | Weaknesses | Opportunities | Threats
--- | --- | --- | ---


