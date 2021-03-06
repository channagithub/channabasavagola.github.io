---
layout: page
title: Projects
jsarr:
 - D3js/pie.js
---

**[Tennis dataset analysis](https://github.com/channabasavagola/australianOpen) using Interactive visualization ([d3.js](https://d3js.org/))**:  
- This is an interactive visualization using d3js. I have used [Sunburst](https://bl.ocks.org/mbostock/4348373) example by [Mike Bostock](https://bl.ocks.org/mbostock) to represent 2008 Australian open matches.
- Size of each partition represents how strong a player is before the match.
- Hover over it to know what round that partition represents.
- This is in continuation to the below static visualization.

<a href="https://channabasavagola.github.io/AustralianOpenInteractiveViz.html">
<img src="/img/interactiveViz.gif" alt="interactiveViz" style="width: 600px;"/>
</a>
	
**[Tennis dataset analysis](https://github.com/channabasavagola/australianOpen) in static visualization ([Tableau public](https://public.tableau.com/profile/channabasava.gola#!/vizhome/10YearsAustralianOpen2008-2017Final/Dashboard1))**:  
- Visualization should speak, not words.

[<img src="/img/viz.png" alt="viz" style="width: 600px;"/>](/img/viz.png)

**[Rainfall prediction](https://github.com/channabasavagola/rainfall-prediction)**:  
- This analysis is part of the research work. Full paper is [here](http://ieeexplore.ieee.org/document/8284469/).  
- Data/feature analysis, feature selection and weather forecasting for Bangalore rainfall based on factors like precipitation, min/max/avg temperature, vapour pressure, cloud coverage, wet day frequency.

<img src="/img/rainfallPredictionImage.png" alt="rainfallPredictionImage" style="width: 700px;"/>

Accordingly to this prediction, rainfall in Bangalore will increase! 
A detailed exploratory data analysis can be found [here](https://github.com/channabasavagola/rainfall-prediction).

**[My chrome browsing history visualization](https://github.com/channabasavagola/myBrowsingAnalysis)**:  
- I have visualized my browsing history. This works for Mac. To make this work on windows, you need to change the path of "History" file.

<img src="/img/myTopBrowsingSites.png" alt="myTopBrowsingSites" style="width: 600px;"/>
<!-- {% for js in page.customjs %}
<script src="//d3js.org/d3.v3.min.js"></script>
<script type="text/javascript" src="../js/pie.js"></script>  
{% endfor %} -->

{% for js in page.jsarr %}
<script src="//d3js.org/d3.v3.min.js"></script>
<script type="text/javascript" src = {{ js }} ></script>
{% endfor %}

My top visited website is Google, because I ask a lot of questions. And second most visited is Gmail, as I'm searching for interenships which is also evident when I see 4, 5, and 7 ranked sites. Third most visited site is [YouTube](https://www.youtube.com/channel/UCv_l4PAiASca3jzSV5NQ2Lg/playlists?view_as=subscriber) from where I learn and watch videos for entertainment.

**[Learning JS](https://github.com/channabasavagola/myBookmarker)**:  
- This is a JavaScript application to bookmark sites, but mainly to learn JS. 

<img src="/img/finalGIF.gif" alt="finalGIF" style="width: 950px;"/>

**Multimedia Web Databases Project**:  
- MWDB academic project which was very interesting to mine the dataset provided. We had MovieLens dataset. Columns were, Movies, there genres, comments, users watched, actors acted. In different data tables. We used TF, TF-IDF to map genres, movies and actors to comments/tag vector space. Then performed statistical analysis to figure out how comments differentiate movies or actors or genres. Then we went on to build recommender system by latent factor analysis, used discriminative (SVD, PCA) and generative (LDA) to calculate implicit ratings and recommend based on the new ratings.
