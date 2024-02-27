# CLUSTERING COUNTRIES :earth_africa:
## WHAT IS A NEIGHBORING COUNTRY IN THIS MODERN GLOBALIZATION ERA

***

What are neighboring countries? The answer seems obvious at first: countries sharing a border. But borders have been slowly getting more complex and even non material. First sea travel, then air travel, then space and the world wide web...

But we can try to discover which countries share some traits, in terms of subjective experiences.

What if a neighborhood of them is just a cluster of countries in which the experience of living is more or less the same, or at least kind of similar?

***

Since the mid 90s, two political scientist, the North american Ronald Inglehart and the german Christian Welzel, tried to organize clusters of countries around two different axis comprehending some country values: one mesuring the ratio of traditional vs secular values, and the other mesuring the ratio of survival vs self expression values.

Their current updated map (from 2020) is the following one:

![alt text](https://github.com/JosepTrota/IRONHACK/blob/main/2022%20-%20(Mar)/Final%20Project/Inglehart%20-%20Welzel%20cultural%20map.jpg?raw=true)

As you can see, there is some criticism to be made:
* The axis consist of somewhat loose features
* There are clear outliers on the clusters
* There is no cluster consistency - they are sometimes geographic, sometimes religious, in previous designs sometimes political...
* Could be ethnocentric or maybe even racist, implying that the countries at the top right have the *correct* values, and the bottom left have the least desirable ones (note that Inglehart is american and Welzel from the western part of Germany, both white males, with high academic profiles, so some bias could be there)

**How can we try to reduce bias and improve the creation of "neighbor countries"?**


***

## The idea

***

To show the most objective clusters possible, but taking into account some subjective data, we can look up some international indexes. We decided to focus on the following ones:

INDEX | SOURCE | POSSIBLE SOURCE BIAS
--- | --- | ---
Inglehart Welzel cultural axis | World Values Survey | inconsistent dimensions, possibly ethnocentrist
Unpeacefulness | Institute for Economics and Peace | tied to the UN, Domestic violence not accounted
Ecological footprint | Global Footprint Network | could understimate overuse of planet's resources (not relevant for this case), seems robust
Education | UNESCO | part of the UN, seems robust
Nominal GDP | International Monetary Fund | much more acurate for industrialized countries
Inequality | CIA World Factbook | tied to US government, gini index used because other indexes (maybe more accurate) have less data
Life expectancy | World Bank | could be ethnocentric, seems robust
Religion | CIA World Factbook | tied to US government, data from minority groups always imputed - lowest value always being 5000
Happiness | World Happiness Report | tied to the UN, possibly ethnocentric, the data is difficult to quantify

Naturally, those sources having bias flags that could threaten the validity of the data is not good, but those are the best sources for each kind of data if we want to have only one source for each feature.

***

## The method

***

After lots and lots of exploratory data analysis and cleaning, we decided to use the KMeans clustering method, trying to use elbow method and silhouette score to validate the number of clusters in each case. It has to be aknowledged that the elbow method rarely gave us relevant information, and we used the silhouette score to decide which was the best number to pick each time.


***

## The results


***

**To see the end product of the project (which is a presentation) go [here](https://slides.com/jostrota/minimal).**

***

The maps with all the clusters can be roughly seen here:

<div class='tableauPlaceholder' id='viz1647554792149' style='position: relative'><noscript><a href='#'><img alt='All clusters ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Cl&#47;Clusteringcountries&#47;Allclusters&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Clusteringcountries&#47;Allclusters' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Cl&#47;Clusteringcountries&#47;Allclusters&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div>               

Or try the [tableau published maps](https://public.tableau.com/app/profile/josep.trota.ochoa.de.eribe/viz/Clusteringcountries/Allclusters?publish=yes).

***

## Later observations and conclusions

***

Conclusions from the data:

* "WESTERN" COUNTRIES (WESTERN EUROPE, CANADA, AUSTRALIA) ARE VERY CONSISTENT: Spain, France, Germany, Norway, Switzerland, Sweden... Seem to consistenly be in the same cluster, very different than any other countires, and always joined by Australia and Canada. Sometimes Japan and the US are in this cluster as well.
* "EASTERN" COUNTRIES ARE USUALLY IN THE SAME CLUSTER: Russia seems to have a tendency to always be in the same neighborhood as some other eastern european countries. Som of those countries in the middle of the east and the west of Europa always seem to pivot between west and east clusters.
* USA AND CHINA - DIFFERENT BUT SIMILAR: They share a cluster only by themselves in the final graphic, and they each have their own lonely cluster in the full dataset clusters (as India does too).
* ALL OTHER COUNTRIES TEND TO BE SCATTERED: other clusters didn't sharea common form in lots of maps, so depending on the data they may differ a lot from each other.


#### FINAL SWOT ABOUT THE PROJECT

Strengths | Weaknesses | Opportunities | Threats
--- | --- | --- | ---
There are lots of important indexes | Data may be easyly unreliable (questionable sources, no data from some countries, the data is from a survey...) | Data improvement can easily lead to cluster improvement | Maybe there was important data left out, or there was some conceptual overfitting... It is difficult to assess.
The use of KMeans reduces the bias | Lots of null values in the data, especially in Africa | Different readings through time can show us growing / shrinking pace of countries, so we could see which countries are *evolving* at similar paces | Subjective data is complex and not easily measured
The final clusters are more complex than the Inglehart Welzel map | Visualization, when having more than 3 dimensions (or worse, more than 5), becomes much harder (it is great to have a map to represent the data in) | | Surveys are not the most objective method
