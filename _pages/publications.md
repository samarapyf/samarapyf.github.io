---
layout: archive
title: "GES 486 Final Project"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
Baltimore: Percent Low Birth Weights by Neighborhood with Known Sources of Air Pollution- A Spatial Analysis
======

Background:

One commonly used measure of health is the birth weight of newborns, as low birth weight is associated with an increased risk of infant mortality, developmental issues, and chronic health problems later in life. Research has shown that exposure to air pollution during pregnancy, particularly fine particulate matter (PM2.5), is associated with decreased birth weight. PM2.5 refers to tiny particles with a diameter of 2.5 micrometers or less, which can penetrate deep into the respiratory system. High levels of PM2.5 have been linked to an increased risk of preterm birth and low birth weight. The exact mechanisms through which air pollution affects birth weight are not fully understood, but it is believed that the inflammation and oxidative stress caused by air pollutants can disrupt placental function, leading to reduced nutrient and oxygen supply to the fetus. Air quality is a major concern for public health, and it is a topic that intersects with social determinants of health, health justice, and health geography. Baltimore is a city that has struggled with air pollution for decades. For my final project I looked at outdoor air quality and pollution and it’s effects on birth weight in Baltimore. The purpose of this project is to highlight the relationship between air pollution and public health in Baltimore.

Data and Methods:

To do this I gathered spatial data about birth weight on the neighborhood scale. I then overlayed that data with known sources of air pollution in Baltimore like major highways and roads, as well as regions zoned as industrial. The map was be created using publicly available data on birth weight in Baltimore, zoning, and transportation routes. I obtained the initial birth weight data from the Baltimore Neighborhood Indicators Alliance (BNIA). The dataset I used was collected in 2019. I downloaded it as a .csv file. In Excel, I added an additional column to show ‘percent babies born below satisfactory weight’, because the original data showed percent born at a satisfactory weight. In addition, the data required spatial information so I also downloaded BNIA’s “Community Statistical Areas” as a GeoJSON file. These community statistical areas are used  to “present a wide range of data from multiple sources as well as providing data for Baltimore City in a consistent way over time” (BNIA). In the QGIS software I joined the tables together, so that the health data had geographic information as well. I added this data to a map, and symbolized it so that it would depict the percent birth weights in a graduated color scheme. In order to depict major highways and roads I used the Quick OSM, or Quick Open Street Map, plugin on QGIS. I entered two queries to retrieve data about both motorways and roads and added that data to my map. I then had to make those queries permanent, or export them as layer files into my map. Lastly, I downloaded data from the Baltimore Department of Planning and downloaded a GeoJSON file that mapped zoning data. I added that file to my map, opened its attribute table, and selected for industrial zones coded, I-1, I-2, and HI. I then exported this selection into a new shapefile and added that to my map to show industrial zones in Baltimore. I then symbolized the map to make it pretty, and made a very pretty and informative layout.

Results and Anaylsis:

According to this data, the neighborhoods Cherry Hill and Southern Park Heights have the highest percentages of low birth weights at 27.8% and 20.2%, respectively (BNIA, 2019). Further, Pigtown and Canton have the lowest percentages of low birth weights at 3.2% and 4.6% (BNIA, 2019). By examining the percentages of low birth weights in Cherry Hill, Southern Park Heights, Pigtown, and Canton, it becomes evident that certain areas have a higher risk of adverse birth outcomes compared to others. 
The goal of this map was to see if there a was a spatial relationship between sources of air pollution and birth weights in Baltimore. With the hopes that a spatial analysis could pinpoint specific areas where interventions and mitigation efforts could be targeted to reduce exposure to harmful pollutants and improve air quality. However, evidence that these sources of air pollution are having a direct impact on birth weights is inconclusive. There is no evident spatial relationship between the neighborhoods with the highest percentages of low birth weights and sources of air pollution. It is likely that in addition to industrial air pollution other social determinants of health such as income, race, and education levels are at play in effecting the uneven results in Baltimore.

Conclusion: 

 Although the results of my hypothesis are unclear, my map appears to tell another story symmetrical with Baltimore’s history of redlining and segregation. There is an evident “white L” and Black butterfly. The term "white L" typically refering to a geographic pattern where predominantly white neighborhoods form an L-shaped region in the northern and western parts of the city, stretching from the downtown area to the northwest. Alternately, the Black Butterfly, coined by Dr. Lawrence Brown, describes two areas of Baltimore with a higher concentration of African American residents. The boundaries of the Black Butterfly are not precisely defined but generally encompass neighborhoods in the eastern and western parts of the city, forming a butterfly wing-like shape of spatial inequality. These patterns of residential segregation and demographic concentration can have significant implications for various aspects of community well-being, including access to resources, education, employment opportunities, and healthcare. Disparities in these areas can contribute to health inequities, social inequalities, and limited economic mobility for certain populations.The goal of this project is to highlight the disproportionate burden of air pollution exposure on low-income communities, communities of color, and communities near industrial sites.
