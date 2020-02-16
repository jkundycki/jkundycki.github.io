---
layout: post
title:      "Project Two: Predicting Real Estate Price"
date:       2020-02-16 13:22:13 -0500
permalink:  project_two_predicting_real_estate_price
---


It feels like it's been forever since the first project but really, it hasn't been that long. Only a month. I feel like my coding skills have improved greatly since then but they are continuously put to the test. Module 2 was all about Statistics. So, naturally, this project was very focused on Statistics. It was also focused on something called OSEMN. What is OSEMN? I'm glad you asked. OSEMN is an acronym that stands for Obtain, Scrub, Explore, Model and Interpret. OSEMN is also the life cycle of Data in Data Science. 
Something we learned how to do in Module 2 was how to create a linear regression model that could predict something based on many different things. Think of the y=mx+b formula you may have learned in Middle School. It's kind of like that but with many mxs. 
Anyway, for the project, we were given a large dataset for houses in King County, Seattle, WA. In the dataset were many features about these houses: bedrooms, floors, square footage, grade,..., and price! The ultimate goal of the project was to build a model that could, as accurately as possible, determine price based on different criteria. To do this, we were advised to follow the path of OSEMN, and that is exactly what I did.

Obtain: This part was the shortest and most straightforward. I was given data and so I imported it. Then I took a look to see where to get started.

Scrub: In data science, you're given a lot of data that has many strange values that don't make much sense to you or the machine. In the cleaning process, decisions need to be made as how to deal with them. In the case of this project, the weird values such as NaN or ? were found in columns that were comprised of 90%+ zeroes. So why not change those strange values to a few more?

Explore: This section has to do with getting familiar with the data and seeing what can be deduced from it. Here I asked questions that I thought were interesting about the data. For example, check out this cool map I made from the latitude and longitude data in terms of price:

<a href="https://ibb.co/BfJ6RcD"><img src="https://i.ibb.co/7SDpFjc/king.jpg" alt="king" border="0"></a>

I also dealt with something called multicolinearity in this section. In layman terms, when building a model, you cannot determine the target (in this case, price) using variables that are related to one another. So, in this instance, the best predictors of price needed to be picked while also not picking intercorrelated variables. 
Below, you can see a heatmap that was made with Seaborn, which is very useful to check multicolinearity:

<a href="https://imgbb.com/"><img src="https://i.ibb.co/KKqh9pp/heatmap.jpg" alt="heatmap" border="0"></a>

Model: This is the part where you build your model, validate that it's a "good" model, and then make some finishing touches.

Interpret: Here you interpret your model. In my case, the model was perfect and I should be hired immediately. But seriously, my model did not look so good in this part. 

When using linear regression, there are assumptions that must be met for you to have a model that can accurately make predictions:

The relationship between the variables and the target should be linear. 
There should be no multicolinearity. 
The residuals of the model should be normal. 
And the residuals of the model should be homoscedastic (even distribution of residuals across the line of best fit, more layman terms). 

Of these my model violated... all of them. Except maybe multicolinearity? Depends who you ask based on the scores I got for the summary of my model. My model also only had 2 features by this point to minimize multicolinearity: square footage of the home and it's latitudinal position which I thought was disappointing; I wish I had had more features.

Despite my model not being what I wanted it to be, the project was very insightful. I must have spent over 60 hours in total working on it and quite frankly, I really enjoyed it. It's heartwarming to have enjoyed it: it reinforces that I made the right decision studying data science. I just hope that the jobs this journey opens up are at least somewhat similar. Just like last time I learned a lot. That being said it's time to put this one to rest. I might keep exploring how to improve this model in my leisure time but I am ready for a much needed break for both my mental and physical health.

I'll see you on the next one.

John
