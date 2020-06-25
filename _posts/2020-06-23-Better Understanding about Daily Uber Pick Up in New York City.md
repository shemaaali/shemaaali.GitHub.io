---
layout: page

cover-img: /assets/img/GettyImages-910282160-1024x683.jpg

tittle: Better Understanding about Daily Uber Pick Up in New York City

subtittle: Better Understanding about Daily Uber Pick Up in New York City

comments: true

tags: [books, test]
---


## Is Uber Making New York City Traffic Worse?



In fact, I wanted to gain a better understanding of daily uber picks up rates in New York City, so I analyzed daily hours rates in a large subset of the busy week-days and weekends. I analysed and visualized all of the available daily uber picks up data, from April 2014 to September 2014.



Using individual daily pick up-level data to answer important questions on pick up sharing services’ influence on markets, drivers, and citizens in New York city by the Data/Time, Lat, Lon, Base, Year, Month, Day of the Weeks, Hours, and Minutes.



## New York City is the Biggest Market for Public Transit in the Country 



New York City is the biggest market for public transit in the country — in fact, about 40 percent of all public transit trips in the United States occur in the New York metro area. And as it happens, we have some very good data on how New Yorkers are using Uber, public transit and other services. Earlier this month, we published an analysis based on about 93 million Uber and taxi trips in New York from April to September 2014, including information about Uber trips that we obtained via a Freedom of Information Law request. That analysis focused mostly on the differences between Uber and taxi coverage: As compared with taxis, for instance, Uber use is proportionally higher in Brooklyn.
But in New York overall, there isn’t much difference between the people picked up by Uber and the ones who ride in cabs. Uber and taxis both disproportionately serve wealthy areas within Manhattan or just across the bridges and tunnels from it. What’s more, these customers usually live in neighborhoods with abundant public transit access also. In other words, the combination of public transit and for-hire vehicles is something that New Yorkers have been relying on for years.
Take a look at the maps we’ve produced below, which track pickups by Uber and taxis on a per capital basis, census tract by census tract. The data includes an adjustment for the ratio of residents to workers in each census tract, with the goal of identifying rides that originate from a person’s place of residence rather than where they work, shop, go to school or spend leisure time.



## New York City is the Biggest Market for Public Transit in the Country Demonstrated By the Following Figure:




![New](http://assets.pewresearch.org/wp-content/uploads/sites/12/2016/04/FT_16.04.06_pubTrans_metro.png)




As you can see, Uber and taxi usage have a lot in common. The correlation coefficient between per capita Uber use and per capita taxi use 3 is 0.89, not that far from a perfect correlation of 1. We can also consider these differences by various geographic and demographic categories on a scale where 100 represents average per capita residential usage.




## The Correlation Coefficient Between Per Capita Uber use and Per Capita Taxi Use As Showed by the Following Figure:




![Correlation](https://tse3.mm.bing.net/th?id=OIP.-MTsh0HdNoNFjZ245TtpzQHaIv&pid=Api&P=0&w=300&h=300)





Uber is introducing some cheaper services, such as its carpooling service UberPool. Suppose that the price of an Uber ride could be halved, to $10 per ride. In that case, this household could take about a third of its trips by Uber, filling in the rest with public transit, and it would still be cheaper than car ownership.





## Cheapest Services Like Carpooling UberPool Illustrated By the Following Figure:





![Cheapest](https://tse4.mm.bing.net/th?id=OIP.ctdk3I3NxPBrg0ANPJVlegHaD3&pid=Api&P=0&w=297&h=156)






## Ubers And Cabs May Not Be So Different In Some Case AS the Following Figure:





![Uber](https://cdn-images-1.medium.com/max/1200/0*V7pDskSARMN3lhSx)




## Uber Can Be Cheaper Than Car Ownershp-If You Mostly Use Puplic Transit



![Uber](https://cdn-images-1.medium.com/max/1200/0*I6GWZa_MXlkkwwJx)



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





