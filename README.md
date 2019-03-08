# US Flight Data Analysis
Analyzed USA’s Domestic flight data of 2017 using Machine Learning techniques to find interesting and rare insights related to flight time, distance and arrival/departure delays. 

## Business Problem

Provide valuable input to customers who need help in choosing the best flight 

Help customers understand which days and months of the week there is a probable chance of delay, which airlines are delayed the most, understanding of how delays differ with flight distance, analysis of delays during departure and arrivals 

## Data Summary:
US domestic flights dataset for the year 2017.

Source – [US Bureau of Transportation](https://www.transportation.gov/).

Contains approx. 6 million records with 70 columns (~2 GB)

## Data Cleaning:
Merging data of each month together.

Replacing null values with appropriate values.

Changing datetimes to proper format ( 1020 -> 10:20:00).

Merging data with geographical co-ordinates

## Insight:
### Would you prefer to choose an airline if you knew that 45% of its flights are delayed?

Probably not ! 

But , through clustering the interesting insight is:

Even though some flights have delayed departures, they still arrive on time or in many cases even before the scheduled arrival time!

![image_descript](/images/1.png)

**Reason:** CRS time adjustment 

![image_descript](/images/2.png)

![image_descript](/images/3.png)

### Predicting arrival delays using regression models:

![image_descript](/images/4.png)

### Steps overview:

1) Used Lasso to find important attributes for prediction.
2) Trained and predicted delays using Lasso Regression Model. (MAD=4.33 mins)
3) Trained and predicted delays using Linear Regression Models. (MAD=3.80 mins)
4) Used Linear Regression Model to predict 2018 quarter 1, delays. (MAD = 3.885 mins)

## Interesting Insights
Shorter distance flights comparatively have more delays than longer distance flights

![image_descript](/images/5.png)

![image_descript](/images/6.png)

![image_descript](/images/7.png)

![image_descript](/images/8.png)


#### On further analysis it can also answer the following questions:

**What is the best season of the year to travel? Flights are delayed usually in which season? Is it in monsoon or winters?**

No, Interesting finding here is that the flights are delayed more in summers than monsoon or winters. The reason is that LOW AIR Density makes it difficult for planes to take off. 

**Are flights more delayed during weekends?**

No, Flights are delayed more during weekdays than weekends.


## Acknowledgments

* [US Bureau of Transportation](https://www.transportation.gov/)

