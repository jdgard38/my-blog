---
layout: post
title:  "Streamlit: a new football app"
author: JD Gardner
description: Come take a look at some football data on an interactive app.   
image: "/assets/images/diving-horse.jpg"
---

## Steps for creating a Streamlit app.  
First thing you want to do when creating a Streamlit app is getting your dataset cleaned and prepped for exploratory data analysis. To do this I scraped a website with data on college football teams. For more information on this refer back to [my last blog post.](https://jdgard38.github.io/my-blog/2025/03/14/Football.html)

After I have my data collected, I can then do some data analysis and see any trends that might be of note. I then create an excel sheet or a comma seperated values(csv), and upload that to a blank code piece. I use this code piece to get into streamlit using the streamlit library or package from python. 
![Header of Code](/assets/images/streamlit_header.png)

## Findings from my Data
I found data that showed how much teams scored in the first week of the 2022 college football season as a home team. Looking through this data and as seen in the streamlit app[(Team Points Distribution)](https://football38.streamlit.app/), the average score for the home team in this first week was 29.97. This number is 1.97 points above 4 touchdowns, which shows that most teams were scoring around 4 touchdowns during their home opener in the 2022 season. 

## My Streamlit app
The purpose of my app is to allow users the access to get on and find their favorite team or conference and see how well they do at home. With multiple different pages and sliders you can navigate the app to show just your favorite conference and see how one specific team did compared to that. There are 3 seperate taps at the top that show: "Conference Analysis", "Team Points Distribution", and "Week Analysis". These tabs all show a broad graph as well with a "Detailed Team Analysis" graph below so that you can see how one team compares to the rest. 

## Why Use my App
My app is very applicable to sports fans, especially college football fans. I will add more data as I get it, and then the app will have even more uses that will show how good college fooball teams have been. For now the app is very useful for looking at how well the home teams do in the first week of the season, and based off my findings looks like majority of the home teams don't have a problem scoring points in their home opener. 

## Ideas for you to use
I encourage all readers here to find a topic they are interested in and find data you can scrape off the web. When scraping data make sure that you do it in a way that is ethical. One way that I like to do it, is by using an API key. This ensures that the website acknowledges you taking their data and is ok with it. After obtaining your data explore it and find creative ways to display it on a streamlit app your self. You can display data in lots of cool ways and not just the same ways that I demonstrated on [my app.](https://football38.streamlit.app/)

Until next time football fans! Keep updating your score books and finding ways that you can become a more invested football fan!!



