---
layout: post
title: Insight Uber Pick Up in New York City 
subtitle: Each post also has a subtitle
gh-repo: shemaaali
/
shemaaali.GitHub.io
gh-badge: [star, fork, follow]
tags: [test]
comments: true
---



Ubers And Cabs May Not Be So Different


![Uber](https://cdn-images-1.medium.com/max/1200/0*V7pDskSARMN3lhSx)



As you can see, Uber and taxi usage have a lot in common. The correlation coefficient between per capita Uber use and per capita taxi use3 is 0.89, not that far from a perfect correlation of 1. We can also consider these differences by various geographic and demographic categories on a scale where 100 represents average per capita residential usage.
Uber is introducing some cheaper services, such as its carpooling service UberPool. Suppose that the price of an Uber ride could be halved, to $10 per ride. In that case, this household could take about a third of its trips by Uber, filling in the rest with public transit, and it would still be cheaper than car ownership.




Uber Can Be Cheaper Than Car Ownershp-If You Mostly Use Puplic Transit

![Uber](https://cdn-images-1.medium.com/max/1200/0*I6GWZa_MXlkkwwJx)


**bold it text**
Insight: Uber Pickup Frequency Based on Hours of the Day
**bold it text**

Uber is mostly busy around 3pm to 9pm and slightly busy in the morning around 6am to 10am.

**bold it text**
Here's a code of Insight: Uber Pickup Frequency Based on Hours of the Day
**bold it text**

~~~
plt.figure(figsize=(15,8))
sns.distplot(uber_april_2014['Hour'])
plt.show()
~~~

**bold it text**
Here's a Graph of Insight: Uber Pickup Frequency Based on Hours of the Day
**bold it text**

![Graph](https://cdn-images-1.medium.com/max/1200/0*ciLYs85OJj2a4UjU.png)

**bold it text**
Insight: Uber Pickup Frequency Based on Days of the Week
**bold it text**

People are choosing uber for weekdays more often then in weekends.

**bold it text**
Here's a code of Insight: Uber Pickup Frequency Based on Days of the Week
**bold it text** 

~~~
plt.figure(figsize=(15,8))
sns.countplot(uber_april_2014['Day_of_week'])
plt.show()
~~~

**bold it text**
Here's a Graph of Insight: Uber Pickup Frequency Based on Days of the Week
**bold it text**

![Graph](https://cdn-images-1.medium.com/max/1200/0*TNVDAc2rDPFx9ydF.png)

**bold it text**
Insight: Unter Base Traffic Monitoring on the Hinter Bases of Day_of_Week and Hours
**bold it text**

It's seem that uber has more pickup on Tuesday wednesday and thusday 
people are opting for uber more in the evening(5pm to 9pm) period than the morning(6am to 9am) and the patter is same throughout the week.

**bold it text**
Here's a code of Insight: Unter Base Traffic Monitoring on the Hinter Bases of Day_of_Week and Hours
**bold it text**

~~~
plt.figure(figsize=(16,8))
sns.countplot(uber_april_2014[uber_april_2014['Base']=='Unter']['Day_of_week'],
              hue=uber_april_2014[uber_april_2014['Base']=='Unter']['Hour'],palette='seismic')
plt.title('Unter Base',size=30)
plt.legend(loc=(1.05,0))
plt.show()
~~~

**bold it text**
Here's a Graph of Insight: Unter Base Traffic Monitoring on the Hinter Bases of Day_of_Week and Hours
**bold it text**

![Graph](https://cdn-images-1.medium.com/max/1200/0*sGsIjPAbQLUOt_x7.png)

**bold it text**
Insight: Hinter Base Traffic Monitoring on the Hinter Bases of Day_of_Week and Hours
**bold it text**

It's seem that uber has less pickup on sunday and monday 
the trend of pickup hour is as similar as observed in Unter traffic analysis.

**bold it text**
Here's a code of Insight: Hinter Base Traffic Monitoring on the Hinter Bases of Day_of_Week and Hours
**bold it text**

~~~
plt.figure(figsize=(16,8))
sns.countplot(uber_april_2014[uber_april_2014['Base']=='Hinter']['Day_of_week'],
              hue=uber_april_2014[uber_april_2014['Base']=='Hinter']['Hour'],palette='seismic')
plt.title('Hinter Base',size=30)
plt.legend(loc=(1.05,0))
plt.show()
~~~

**bold it text**
Here's a Graph of Insight: Hinter Base Traffic Monitoring on the Hinter Bases of Day_of_Week and Hours
**bold it text**

![Graph](https://cdn-images-1.medium.com/max/1200/0*W1EP0Dq27-k3g7Zn.png)

**bold it text**
Coding
**bold it text**
I have limited experience in coding: Some foundation in Python and very limited machine learning. But I'm lucky to have the chance to do a bit development with ipynb, so I have enough to start building an environment coding page with python.


