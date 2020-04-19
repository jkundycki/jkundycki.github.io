---
layout: post
title:      "Project Four: Building a Movie Recommender System"
date:       2020-04-19 22:21:10 +0000
permalink:  project_four_building_a_movie_recommender_system
---

<a href="https://ibb.co/jk2s1nn"><img src="https://i.ibb.co/TMSdF99/Netflix.png" alt="Netflix" border="0"></a><br /><a target='_blank' href='https://imgbb.com/'>img hosting</a><br />

For those of us constantly accessing the web, we are all too familiar with Recommender Systems. They are all around us and are either those pesky ads that are listening in on our conversations or a holy grail for new information or purchases. Love them or hate them, these recommender systems are widespread for a reason. These systems have played an integral part in the success of many large online businesses such as Amazon, Google and Spotify and are providing some of these companies up to 30% of their total revenue. 

The goal of this project is to build a basic recommender model to get more familiar with aspects of Machine Learning. To  achieve this goal, the popular online movie dataset from MovieLens has been employed to make movie recommendations to users based on how they rate certain movies. The MovieLens dataset contains over 100,000 real world ratings for many different films and many different users. The dataset was produced by having volunteers rate movies on a scale from 1-5 based on how they enjoyed the movie.

The way the model works is by having users start by rating several films to "put them on the map" in terms of data, handling what is called the cold approach. The movies suggested to the users will be based on movies that similar users enjoyed (users who rated movies similarly to those being suggested to), also known as collaborative filtering. The model in this project was produced using Alternating Least Squares in PySpark.

To further challenge myself, I decided to try and modernize the rating system. For those familiar with Spotify, Netflix or any popular entertainment platform with a recommender system, you will know that these days, the thumbs up or thumbs down is the way to rate content. These platforms have moved to this system because it has greatly improved the accuracy of predictions for users. I modernized my recommender model by changing the ratings to either a 1 (thumbs up) or 0 (thumbs down). 

<a href="https://ibb.co/LPz5MjC"><img src="https://i.ibb.co/ZJ6m34h/binary.jpg" alt="binary" border="0"></a><br /><a target='_blank' href='https://imgbb.com/'>img hosting</a><br />

The model could still use some tuning to become a better predictor and I would like to create a GUI so that anyone could interact with the model in an intuitive way and receive movie recommendations.

Thanks for reading and best of luck to you,

John
