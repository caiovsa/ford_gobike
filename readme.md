# Ford GoBike System Data Exploration and Visualization
## by Caio Vasconcelos

<!---![stack Overflow](https://nextcity.org/images/daily/_resized/fordgobike.jpg) -->

<p align="center">
  <img src="https://nextcity.org/images/daily/_resized/fordgobike.jpg" width="925" title="hover text">
</p>

## Dataset

>  This notebook explores a dataset about the Ford Gobike system, a bike-sharing system covering the greater San Francisco Bay area, now know as Bay Wheels. 
The bicycles are available 24 hours a day, seven days a week for periods ranging from a single ride (up to 30 minutes) to a day pass, in 30-minute increments,
or customers can purchase an annual subscription which gives them unlimited rides up to 45-minutes in duration. Single rides cost $2 per trip, day passes cost $10 per day, 
and memberships cost $15 per month or $149 per year.
 
> The dataset counts with 183412 values with features like gender, stations name and other ones

> Data wrangling:

> * The dataset was provided by Udacity;
> * Changed the columns start and end time to datetime;
> * The dataset have 16 columns, and we created another one with the days of the week, exctracted from the start_time column!;
> * Filter out outlier birth years;
> * Filter out outlier trip durations when the duration was too long!

## Summary of Findings

> There are mainly two tipes of users in this service, the normal Costumer and the Subscriber.
 The service is mainly used through the work days and declines in the weekends. 
 Another intersting factor is the age (20 - 40 years old) and the duration of the trips, 85% of the trips take less then 1000 seconds ( less then 15 minutes)!
 
### Main aspects:
* There were more trips on work days compared to weekends. 
* The duration in secs of the trips are most of them in between 200 to 1000...meaning that most trip are less then 15 minutes! Which makes a lot of sense because this service works with single rides (up to 45 minutes to Subscribers);
* Most users were male. 
* We had a lot more subscribers then normal customers 
* The most common age was around 20 to 40 years old (1980 - 2000). Older people tend to uset it a lot less than the younger ones too.
* The most used start stations ( Where the person rented the bike) were almost the same as the most used end station ( Where the person leaves the bike). Must of the bike trips should have been in between then!
* The numbers of Male users were a lot more expressive then womens. But womens had longer trips!



## Key Insights for Presentation

> We have a different usage for both the Subscriber and the Normal Costumer. 
While the Subscriber uses the service most of the time on work days (Monday trough Friday), 
the normal Costumer uses it more on the weekends including Friday! 
The normal Costumer must be someone that is using the service for fun, rather than addopting 
it like a way of transportation, so the costumer must be someone like a turist exploring the 
Bay area, and the Subscriber is someone that uses the service more recurring like someone that 
uses it daily to go to universty or maybe work! The short period of usage by both is very intersting too, showing that the most used stations must be very near of one another.