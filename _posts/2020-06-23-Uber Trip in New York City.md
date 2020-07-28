---
layout: post

tittle: Prescription Drug Abuse In The United States

subtittle: What Should We Do To Prevent Prescription Drug Abuse?

cover-img: /assets/img/

tags: [books, test]

comments: true
---


## Is Uber Making New York City Traffic Worse?



In fact, I wanted to gain a better understanding of daily uber picks up rates in New York City, so I analyzed daily hours rates in a large subset of the busy week-days and weekends. I analysed and visualized all of the available daily uber picks up data, from April 2014 to September 2014.



This post shows using individual daily pick up-level data to answer important questions on pick up sharing services’ influence on markets, drivers, and citizens in New York city by the Data/Time, Lat, Lon, Base, Year, Month, Day of the Weeks, Hours, and Minutes.




## New York City is the Biggest Market for Public Transit in the Country 


New York City is the biggest market for public transit in the country contents about 40 percent of all public transit trips in the United States occur in the New York metro area. we published an analysis based on about 93 million Uber and taxi trips in New York from April to September 2014. We can compare between taxis and uber using high proportion is in Brooklyn. They might be a lot different between people who ride uber or taxi.



There are some cheaper services for uber like UberPool. The price of ride is between $8-$10.


## Cheapest Services for uber like UberPool Illustrated By the Following Figure:




![Cheapest](https://tse4.mm.bing.net/th?id=OIP.ctdk3I3NxPBrg0ANPJVlegHaD3&pid=Api&P=0&w=297&h=156)




## Insight: Uber Pickup Frequency Based on Hours of the Day



Uber is mostly busy around 3pm to 9pm and slightly busy in the morning around 6am to 10am.



## Here's a code of Insight: Uber Pickup Frequency Based on Hours of the Day






~~~
plt.figure(figsize=(15,8))
sns.distplot(uber_april_2014['Hour'])
plt.show()
~~~








## Here's a Graph of Insight: Uber Pickup Frequency Based on Hours of the Day




![Graph](https://cdn-images-1.medium.com/max/1200/0*ciLYs85OJj2a4UjU.png)




## Insight: Uber Pickup Frequency Based on Days of the Week



People are choosing uber for weekdays more often then in weekends.



## Here's a code of Insight: Uber Pickup Frequency Based on Days of the Week








~~~
plt.figure(figsize=(15,8))
sns.countplot(uber_april_2014['Day_of_week'])
plt.show()
~~~








## Here's a Graph of Insight: Uber Pickup Frequency Based on Days of the Week



![Graph](https://cdn-images-1.medium.com/max/1200/0*TNVDAc2rDPFx9ydF.png)



## Insight: Unter Base Traffic Monitoring on the Hinter Bases of Day_of_Week and Hours


It's seem that uber has more pickup on Tuesday wednesday and thusday 
people are opting for uber more in the evening(5pm to 9pm) period than the morning(6am to 9am) and the patter is same throughout the week.


## Here's a code of Insight: Unter Base Traffic Monitoring on the Hinter Bases of Day_of_Week and Hours








~~~
plt.figure(figsize=(16,8))
sns.countplot(uber_april_2014[uber_april_2014['Base']=='Unter']['Day_of_week'],
              hue=uber_april_2014[uber_april_2014['Base']=='Unter']['Hour'],palette='seismic')
plt.title('Unter Base',size=30)
plt.legend(loc=(1.05,0))
plt.show()
~~~








## Here's a Graph of Insight: Unter Base Traffic Monitoring on the Hinter Bases of Day_of_Week and Hours



![Graph](https://cdn-images-1.medium.com/max/1200/0*sGsIjPAbQLUOt_x7.png)



## Insight: Hinter Base Traffic Monitoring on the Hinter Bases of Day_of_Week and Hours



It's seem that uber has less pickup on sunday and monday 
the trend of pickup hour is as similar as observed in Unter traffic analysis.



## Here's a code of Insight: Hinter Base Traffic Monitoring on the Hinter Bases of Day_of_Week and Hours







~~~
plt.figure(figsize=(16,8))
sns.countplot(uber_april_2014[uber_april_2014['Base']=='Hinter']['Day_of_week'],
              hue=uber_april_2014[uber_april_2014['Base']=='Hinter']['Hour'],palette='seismic')
plt.title('Hinter Base',size=30)
plt.legend(loc=(1.05,0))
plt.show()
~~~






## Here's a Graph of Insight: Hinter Base Traffic Monitoring on the Hinter Bases of Day_of_Week and Hours




![Graph](https://cdn-images-1.medium.com/max/1200/0*W1EP0Dq27-k3g7Zn.png)




# Coding:

I have limited experience in coding: Some foundation in Python and very limited machine learning. But I'm lucky to have the chance to do a bit development with ipynb, so I have enough to start building an environment coding page with python.



# Resources


https://fivethirtyeight.com/


# Addition Resources If Interested


https://medium.com/data-tale/is-uber-taking-over-new-york-city-faf9e03d4c34

https://search.yahoo.com/search?fr=mcafee&type=E211US714G0&p=Uber+pick+up+in+New+york+city



