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

is residential area surrounded by nature, e.g. park, forest, lake
is within reach to daily essential places e.g. market places, pharmacies, public transport
lower population density; area with high population density is perceived low safety and environmental quality
affordable housing price; price should be affordable for young families to get mortgage to finance the house
more modern houses; assume that old houses might require renovation hence increase the cost
I understood that the criteria above may not reflect bigger population. However, in my opinion, the above categories could fit the stakeholders who just start their professional career.

This assignment will showcase data science tools and knowledge I have gained to generate a few most promising neighborhoods based on the above criteria. Advantages of each area will then be clearly expressed so that best possible final location can be chosen by stakeholders.


---

###### Important Note: Using pop() on a Set in Python

In the real world - we would need to make a consideration around the pop() method when used on a Set as in some cases it can be a bit inconsistent.

The pop() method will usually extract the lowest element of a Set. Sets however are, by definition, unordered. The items are stored internally with some order, but this internal order is determined by the hash code of the key (which is what allows retrieval to be so fast). 

This hashing method means that we can't 100% rely on it successfully getting the lowest value. In very rare cases, the hash provides a value that is not the lowest.

Even though here, we're just coding up something fun - it is most definitely a useful thing to note when using Sets and pop() in Python in the future!

The simplest solution to force the minimum value to be used is to replace the line...

```ruby
prime = number_range.pop()
```

...with the lines...

```ruby
prime = min(sorted(number_range))
number_range.remove(prime)
```

...where we firstly force the identification of the lowest number in the number_range into our prime variable, and following that we remove it.

However, because we have to sort the list for each iteration of the loop in order to get the minimum value, it's slightly slower than what we saw with pop()!


