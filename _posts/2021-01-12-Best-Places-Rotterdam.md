---
layout: post
title: Best Places to Live in Rotterdam
image: "/posts/Rotterdam-GettyImages.jpg"
tags: [Python, API web scraper, Geoencoder, KMeans]
---

This is basically the Capstone Project I developed in December 2020 as requirement to get the IBM Data Science Professional Certificate on Coursera, the program which has provided me a strong foundation to pivot to Data Science field. The subject is so dear to me due to many reasons. Not only because Rotterdam is one of my favorite's city in the world; the people, the vibe, the architecture; but also the concerns we have in the society about how difficult it is to find to best place to live in the hustle-bustle of big cities. This project I hope will shine a light to young professionals with limited budget who want to find the best place to call it a home in the-what-so-called, *the Manhattan at the Meuse*.

Let's get into it!

---

### Introduction: Business Problem 

Rotterdam is well-known as a major logistic and economic center and has Europe's largest seaport. It is the 2nd largest city and minicipality in The Netherlands. With a population of more than 650,000 living in an area of 324 km2, Rotterdam is known for its university, riverside setting, lively culture life, maritime heritage and modern culture, and not to forget, it is a home to over 180 nationalities [1].

Having a plan to look for real estate in Rotterdam, I decided to analyse Rotterdam for this project. I am particularly interested in having the knowledge of where the best place to live in this city. In my opinion, the best place to live can be defined as the neighborhood which:

1. is residential area surrounded by nature, e.g. park, forest, lake
2. is within reach to daily essential places e.g. market places, pharmacies, public transport
3. lower population density; area with high population density is perceived low safety and environmental quality
4. affordable housing price; price should be affordable for young families to get mortgage to finance the house
5. more modern houses; assume that old houses might require renovation hence increase the cost

I understood that the criteria above may not reflect bigger population. However, in my opinion, the above categories could fit the stakeholders who just start their professional career.

This assignment will showcase data science tools and knowledge I have gained to generate a few most promising neighborhoods based on the above criteria. Advantages of each area will then be clearly expressed so that best possible final location can be chosen by stakeholders.

---

### Data 
Based on definition of the problem, factors that may influence stakeholder's decision are:

* location
* population density
* average house price
* age of the house

The following data sources will be neede to extract and generate the required information:

* list of neighborhoods in Rotterdam, its population density, age of houses in the area and the average house prices can be obtained from PDOK, a data platform for accessing geo data sets of Dutch governments [2]
* number of venues, their type and location in every neighborhood will be obtained using Foursquare API
* geospatial coordinate of neighborhoods in Rotterdam will be obtained by using Geocoder Python package



