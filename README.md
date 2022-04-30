# Analysis Overview

A famous and well respected Hawaiian surfer named W. Avy has agreed to help me with a business idea: a surf shop on the island of Oahu that also sells ice cream. He needed my help analyzing the different weather trends on the island so that we can make good business decisions that will help us thrive when we open up this shop. In order to determine if this shop will be sustainable year round, I've been asked to analyze the weather data for the months of June and December. There were two deliverables that I completed:

* Deliverable 1 : Determine the Summary Statistics for June
* Deliverable 2: Determinee the Summary Statistics for December

I used the VScode application to write my python codes with the help of my imports: numpy, sqlalchemy and pandas.

# Deliverable 1 Results

I began this deliverable by writing a query that filtered the Measurement table to retrieve the June temperatures on the island. Prior to this, an engine was created with the provided file titled "hawaii.sqlite." This file contains two tables: "measurement" and "station."
To write this query, I declared a new variable called "results" and I executed a session query on the Measurement table extracting the month that is equal to 6 (June). This line of code looks like this:
<img width="885" alt="Screen Shot 2022-04-30 at 12 23 29 PM" src="https://user-images.githubusercontent.com/100390727/166115879-3a8d4bb7-f27c-4054-9636-cbcb7c681d09.png">
These temperatures were then converted to a list, and when I displayed the list by printing "results," we can see the many dates in the month of June contained in a list.
Then, I used pandas to create a dataframe with 2 column names, "date" and "June Temps." 
I used the "describe()" function to display the summary statistics for this dataframe. Here's what I found:

* There were a total of 1700 temperatures recorded for the month of June.
* The average temperature in Oahu for the month of June is 74.94 degrees Ferenheit. This is a nice, warm temperature and ideal for operating our shop.
* The maximum temperature is 85 degrees, and the minimum temperature is 64 degrees for the month of June.
<img width="207" alt="Screen Shot 2022-04-30 at 12 29 09 PM" src="https://user-images.githubusercontent.com/100390727/166116082-04cc1006-2af6-4848-8dc2-047b95616e9d.png">

# Deliverable 2 Results

This deliverable was basically identical to the first one, with the difference being that instead of looking at June temperatures, I analyzed temperatures in December. I first ran a session query on the measurement table to retrieve the December temperatures. I converted these temperatures to a list and then used pandas to create a dataframe of this data. The labeled the two columns "date" and "December Temps." 
Then, just like with the June temperatures, I used "describe()" to get the summary statistics. Here's what I found:

* There were a total of 1517 temperatures recorded for the month of December.
* The average temperature in Oahu  is 71.04 degrees for December.
* The maximum temperature is 83 degrees and the minimum is 56 degrees.
<img width="201" alt="Screen Shot 2022-04-30 at 12 35 08 PM" src="https://user-images.githubusercontent.com/100390727/166116233-85cae3fd-fae9-403d-87be-c201fae68711.png">

# Summary

After completing the two deliverables, I'm feeling very good about opening up this surf/ ice cream shop. The average temperature for June is only around 3 degrees hotter than the average temperature of December. This means that the weather appears to always be quite nice on this island. According to our data, we don't have a recorded day in June that is above 85 degrees, and the highest temperature in December is 83 degrees. This is spectacular ice cream weather! I do have a bit of surfing knowledge and I do know that the amount of wind plays a big part in weather or not surfers are out on the ocean. If possible, I would like to analyze the wind data for these two months as well to determine how many days would actually be ideal for surfing. I would also like to analyze the data of neighboring ice cream shops and surf shops to see what our competition would be, or to get a better idea of how popular these places are in the neighborhood.
All in all, I'm glad I was able to help my friend W. Avy with this data analysis. I'm already starting to pack my bags and make arrangements so I can live the island life as soon as possible. Surfs up!

