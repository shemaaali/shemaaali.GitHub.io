---
layout: post
title: Is Uber Making New York City Traffic Worse?
subtitle: Using Individual Daily Pick Up
cover-img: /assets/img/https://cdn-images-1.medium.com/max/1200/0*VQlNuAz-phPQ-VnV.jpeg
tags: [books, test]
---

Using individual daily pick up-level data to answer important questions on pick up sharing services’ influence on markets, drivers, and citizens in New York city by the Data/Time, Lat, Lon, Base, Year, Month, Day of the Weeks, Hours, and Minutes.

In fact, I wanted to gain a better understanding of daily uber picks up rates in New York City, so I analyzed daily hours rates in a large subset of the busy week-days and weekends. I analysed and visualized all of the available daily uber picks up data, from April 2014 to September 2014.

New York City is the biggest market for public transit in the country — in fact, about 40 percent of all public transit trips in the United States occur in the New York metro area. And as it happens, we have some very good data on how New Yorkers are using Uber, public transit and other services. Earlier this month, we published an analysis based on about 93 million Uber and taxi trips in New York from April to September 2014, including information about Uber trips that we obtained via a Freedom of Information Law request. That analysis focused mostly on the differences between Uber and taxi coverage: As compared with taxis, for instance, Uber use is proportionally higher in Brooklyn.
But in New York overall, there isn’t much difference between the people picked up by Uber and the ones who ride in cabs. Uber and taxis both disproportionately serve wealthy areas within Manhattan or just across the bridges and tunnels from it. What’s more, these customers usually live in neighborhoods with abundant public transit access also. In other words, the combination of public transit and for-hire vehicles is something that New Yorkers have been relying on for years.
Take a look at the maps we’ve produced below, which track pickups by Uber and taxis on a per capital basis, census tract by census tract. The data includes an adjustment for the ratio of residents to workers in each census tract, with the goal of identifying rides that originate from a person’s place of residence rather than where they work, shop, go to school or spend leisure time.

As you can see, Uber and taxi usage have a lot in common. The correlation coefficient between per capita Uber use and per capita taxi use3 is 0.89, not that far from a perfect correlation of 1. We can also consider these differences by various geographic and demographic categories on a scale where 100 represents average per capita residential usage.

Uber is introducing some cheaper services, such as its carpooling service UberPool. Suppose that the price of an Uber ride could be halved, to $10 per ride. In that case, this household could take about a third of its trips by Uber, filling in the rest with public transit, and it would still be cheaper than car ownership.

Insight: Uber Pickup Frequency Based on Hours of the Day
Uber is mostly busy around 3pm to 9pm and slightly busy in the morning around 6am to 10am.


plt.figure(figsize=(15,8))
sns.distplot(uber_april_2014['Hour'])
plt.show()

Insight: Uber Pickup Frequency Based on Days of the Week
People are choosing uber for weekdays more often then in weekends.


plt.figure(figsize=(15,8))
sns.countplot(uber_april_2014['Day_of_week'])
plt.show()

Insight: Unter Base Traffic Monitoring on the Hinter Bases of Day_of_Week and Hours
It's seem that uber has more pickup on Tuesday wednesday and thusday
people are opting for uber more in the evening(5pm to 9pm) period than the morning(6am to 9am) and the patter is same throughout the week.


plt.figure(figsize=(16,8))
sns.countplot(uber_april_2014[uber_april_2014['Base']=='Unter']['Day_of_week'],
              hue=uber_april_2014[uber_april_2014['Base']=='Unter']['Hour'],palette='seismic')
plt.title('Unter Base',size=30)
plt.legend(loc=(1.05,0))
plt.show()

Insight: Hinter Base Traffic Monitoring on the Hinter Bases of Day_of_Week and Hours
It’s seem that uber has less pickup on sunday and monday
the trend of pickup hour is as similar as observed in Unter traffic analysis.

plt.figure(figsize=(16,8))
sns.countplot(uber_april_2014[uber_april_2014['Base']=='Hinter']['Day_of_week'],
              hue=uber_april_2014[uber_april_2014['Base']=='Hinter']['Hour'],palette='seismic')
plt.title('Hinter Base',size=30)
plt.legend(loc=(1.05,0))
plt.show()

Coding
I have limited experience in coding: Some foundation in Python and very limited machine learning. But I’m lucky to have the chance to do a bit development with ipynb, so I have enough to start building an environment coding page with python.
