---
layout: post

tittle: Prescription Drug Abuse In The United States

subtittle: What Should We Do To Prevent Prescription Drug Abuse?

cover-img: /assets/img/0_qa-FbC-ReXxKIntl.jpg

tags: [books, test]

comments: true
---


## What Should We Do To Prevent Prescription Drug Abuse?



In fact, the abuse of prescription drugs is a common problem in the United States among teens and adult people. Some people use prescriptions as medications, but some people use them as recreational drugs. Millions of dollars are spent to prevent prescription drug abuse, and pharmaceutical companies could make medications have less addictive chemicals. It may take more than is needed, and people may become addicted to prescription drugs.


## When Does It Occur? 


Prescription drug abuse occurs when people who have problems with pain and anxiety take more medications than prescribed, or they take medications not prescribed. People think that if one pill helps, two or more benefits more. Other people try to prevent problems by taking medications before the pain comes. Sometimes medications seem to be the only thing that makes somebody feel better, but many people are not aware of the risks of prescription drug abuse.



## The Dangers and Negative Consequences of Prescription Drug Abuse:



Prescription drugs are called Opioids which are easier to obtain than illegal drugs such as heroin and cocaine. Opioids are prescribed primarily as pain relievers despite a high risk of addiction and overdose. The increase in deaths caused by the risks involved with the consumption of opioids was alarming and declared an epidemic. When those prescription drugs/opioids are taken abnormally, they may result in death and lead to a crisis. 


## Prescription Drug Abuse/Opioid Crisis:


According to CDC, there are more than 750,000 people have died since 1999 from a drug overdose, and there are two out of three drug overdose deaths in 2018 involved an opioid, including prescription opioids, heroin. https://www.cdc.gov/drugoverdose/data/index.htm
In fact, I wanted to gain a better understanding of the prescription drug abuse/opioid crisis, so I analyzed the amount of obtaining a prescription/opioid in a large subset of the data on prescribers like specialties who have authorized the count of each drug are people used. I analyzed and visualized all of the available prescription drug abuse/opioid crisis by https://github.com/IBM/predict-opioid-prescribers/tree/master/data
My primary goal is to perform an exploratory data analysis on the prescription drug abuse/opioid crisis and gather insights into its sources.




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



