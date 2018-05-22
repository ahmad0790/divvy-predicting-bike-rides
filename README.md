# Predicting departures and arrivals by hour for each station for Chicago's Bike Sharing System

Divvy is Chicago's bike sharing system since 2013. Conveniently, Divvy also captures all trip data on its website. https://www.divvybikes.com/system-data. One of the main problems with Divvy is that sometimes on certain hours of the day stations can either get full or empty. This is a pain point for riders who either can't find a bike or can't dock when they have to leading to overtime fees (or being late to work yikes!). To overcome this problem, divvy manages a series of re-balancer vans that are moving around the city during the day to pick excess bikes from full stations and then placing them at stations where there are few or no bikes but great demand. This is a manual process based on past driver experience.

The goal of the workbooks here was to see if Divvy data could be used to predict how many bikes were expected to arrive and depart for each hour of each day and at each of the almost 600 stations scattered across the city. If we could predict beforehand the demand at each station then divvy rebalancer vans could move around the city addressing this demand as this would tell them which stations would get full or empty.

In these workbooks, I use divvy data to help build simple regression models on 2016 data using features engineered from 
1) the weather 
2) historical station activity 

to predict the number of arrivals and departures at each station during each hour of the day. I then evaluate the model performance on out of test 2017 data, and slice it by different features to see how well the model is performing.

Update: the City of Chicago recently released data which has number of bikes available and not available by station every 10 minutes. This data can be extremely predictive and will be added in to the analysis to see if it improves model performance.
