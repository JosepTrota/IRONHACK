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

Of course, those sources have multiple bias flags that could threaten the validity of the data, but those are the best source for each kind of data, if you want to take the same metrics for a feature from the same place.

***

## The method

***

After lots and lots of exploratory data analysis and cleaning, we decided to use the KMeans clustering method, trying to use elbow method and silhouette score to validate the number of clusters in each case. We must say that the elbow method rarely gave us relevant information, and we used the silhouette score to decide which was the best number to pick.


***

## The results

***

The maps with all the clusters can be seen here:

<div class='tableauPlaceholder' id='viz1647550742432' style='position: relative'><noscript><a href='#'><img alt='All clusters ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Cl&#47;Clusteringcountries&#47;Allclusters&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Clusteringcountries&#47;Allclusters' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Cl&#47;Clusteringcountries&#47;Allclusters&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1647550742432');                    var vizElement = divElement.getElementsByTagName('object')[0];                    if ( divElement.offsetWidth > 800 ) { vizElement.style.width='1420px';vizElement.style.minHeight='287px';vizElement.style.maxHeight='987px';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='1420px';vizElement.style.minHeight='287px';vizElement.style.maxHeight='987px';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else { vizElement.style.width='100%';vizElement.style.height='1577px';}                     var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

For further explanation, and to see the end product of the project, which is a presentation, go [here](https://slides.com/jostrota/minimal).

***

## Later observations and conclusions

***



#### SWOT ABOUT THE PROJECT

Strengths | Weaknesses | Opportunities | Threats
--- | --- | --- | ---


