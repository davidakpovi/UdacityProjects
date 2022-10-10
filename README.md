# Fordgobike-Tripdata Exploration
## by David G. AKPOVI


## Dataset

The dataset I choose is called Fordgobike-Tripdata. This dataset includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. Fordgobike-Tripdata is a bike-sharing system where people can borrow a bike to go where they want. They can be customer or subscriber.
The dataset can be found here :  https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv. 

Before doing my exploration, I have done some data wrangling:

- I have deleted null values
- I have changed the types of start_time, end_time, user_type, member_gender and    	
  bike_share_for_all_trip
- I deleted the columns start_station_latitude, start_station_longitude, end_station_latitude, 
  end_station_longitude. I judged them useless for my exploration
- I added a new column called “age” to facilitate my visualization and changed its type
- I limited the ages of user people to 90 years old to not have outlines values 





## Summary of Findings



For my exploration, I choose two features of interest : duration and user type. To have a more clear visualization, I converted the duration in seconds into minutes. I have done univariate, bivariate and multivariate exploration. These explorations helped me to have these findings : 

- The duration of most of the bike trips doesn’t last more than 30 mn
- There are more males users for this service than females
- Thursday is the day of the week where the service is more used
- The duration of the trip for customer is more than subscribers duration
- Males service usage duration is less than females usage duration which is less than other gender duration.
- There are more subscribers than customers for every genders
- Customers and subscribers have approximately the same ages
- Subscribers take less time every days of the week, compared to the customers.



## Key Insights for Presentation



  - The duration of most of the bike trips doesn’t last more than 30 mn 
Duration of a trip is an important data for the bike trip service. I focused on it to know the average. In this dataset, the duration was in seconds. When I tried to do an univariate exploration, it showed me a visualization which was hard to interpret. I had to convert the duration in seconds into minutes. To do that, I divide the duration by 60. The visualization I obtained was more cleared. It showed me that more than 160000 users have bike ride duration between, approximately, 1 mn and 23 mn. Most of the trip bike don’t exceed more than 30 mn. 



  - The bike trip service has more subscribers than customers. 

I found this data very important for this service because it is essential to know what people use the service. To find out, I used a “countplot” with user type as variable. It showed me that approximately 160000 people are subscribers and less than 20000 people are customers. 


- All genders subscribers have less service usage duration in minutes than customers.

To find out this data, I used a multivariate exploration between member_gender, duration_min and user_type. It gave a data visualization in two parts. One part showed the duration in minutes for customers of all genders and the other part showed the duration in minutes for subscribers. We can see on the visualization that for customers, duration for male is approximately 20 minutes, 23 minutes for females and more than 25 minutes for other genders. For subscribers, males average duration is less than 10 minutes, for females is a little above than 10 minutes and for the other is approximately 15 minutes. 