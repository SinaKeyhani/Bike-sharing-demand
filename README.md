# Bike Sharing Demand Prediction🚴🏻

<p align="center">
<img src="https://raw.githubusercontent.com/SinaKeyhani/Bike-sharing-demand/main/borisbike.avif" alt="Project Image" width="400" height="300"/>
</p>

## Introduction
Bike-sharing systems are a modern twist on bike rentals, with everything automated from sign-up to return. Users can easily grab a bike at one spot and drop it off at another. They're becoming popular because they help with traffic, the environment, and health.

This dataset offers key details about bike rentals, including factors like date and time, weather, and holidays. It provides hourly rental data over a two-year period. For this competition, the training set includes data from the first 19 days of each month, while the test set covers the 20th to the end of the month.

Dataset : https://www.kaggle.com/c/bike-sharing-demand/data

## Objective: 
This project uses regression algorithms to predict the hourly bike rental counts in the test set based on prior data. We'll evaluate models using the Root Mean Squared Logarithmic Error (RMSLE) to choose the most accurate one.

## Features:

                  | Variable      | Description                                                                                                 |
                  | ------------- | ----------------------------------------------------------------------------------------------------------- |
                  | id            | A notation for a house                                                                                      |
                  | season        | 1 = Winter, 2 = Spring, 3 = Summer, 4 = autumn                                                              |
                  | holiday       | 1 = holiday, 0 = not holiday                                                                                |
                  | workingday    | 1 = working day, 0 = not working day                                                                        |
                  | weather       | 1 = Clear, 2 = Cloudy, Mist, 3 = Snow,4 = Heavy Rain                                                        |
                  | temp          | temperature in Celsius                                                                                      |
                  | atemp         | "feels like" temperature in Celsius                                                                         |
                  | floowindspeedr| wind speed                                                                                                  |
                  | casual        | number of non-registered user rentals initiated                                                             |
                  | registered    | number of registered user rental initiated                                                                  |
                  | count         | number of total rentals                                                                                     |

## Approach: 
Spent much time dealing with exploratory data analysis and feature selection before fitting data into the model. Tried three different models, Linear Regression and Random Forest and Decion tree and then by using Root Mean Squared Logarithmic Error (RMSLE) measured the model performance.


## Installation & Usage
To run this project locally, follow these steps:

1. Ensure Python is installed on your machine.
2. Clone this repository
   ```
    git clone https://github.com/SinaKeyhani/Buke-sharing-demand/tree/main
   ```
3. Install the required Python libraries for this project.

## Analytical Methods & Visualisation
1. Analysing the effect of weather conditions on the demand in different hours
<p align="center">
<img src="https://github.com/SinaKeyhani/Bike-sharing-demand/blob/main/output.png" alt="Project Image" width="600" height="700"/>
</p>

The demand for bike rentals at different hours is directly influenced by weather conditions. Specifically, we observe a significant increase in demand during periods of favorable weather, particularly between 7 to 8 AM and from 5 to 8 PM. These times consistently show high demand when the weather is clear and pleasant.

2. Analysing hour of the day for different Seasons 
<p align="center">
<img src="https://github.com/SinaKeyhani/Bike-sharing-demand/blob/main/Hour%20vs%20mean%20count%20for%20seasons.png" alt="Project Image" width="600" height="500"/>
</p>

It's evident that peak hours for bike rentals remain consistent across seasons, likely due to work-related commuting patterns that persist regardless of the time of year. 
Interestingly, despite the consistent peak hour trend, Winter stands out with lower bike rental counts. This divergence could be attributed to the prevalence of cold conditions during ths Season.

3. Comparing demands between subscriber and pay as you go customers by days
<p align="center">
<img src="https://github.com/SinaKeyhani/Bike-sharing-demand/blob/main/subscriber%20vs%20Casual%20customers%20by%20weeks.png" alt="Project Image" width="600" height="500"/>
</p>

This graph illustrates the difference in demand between subscribers and casual customers. It is clear that subscribers tend to use the service more during the weekdays, likely due to work or school commitments. In contrast, casual customer demand is higher on weekends. This pattern suggests that targeting casual customers with marketing strategies during weekdays could be an effective tactic for converting them into subscribers.

## Conclusion
Our data preparation and analysis process has provided valuable insights and led to effective model implementation. We meticulously refined the dataset by converting datetime formats, replacing categorical values, and addressing anomalies in variables such as humidity and wind speed. This groundwork paved the way for accurate analysis and model training.

Through exploratory data analysis, we identified key trends and patterns. We found that bike rental counts are higher on weekdays compared to weekends and holidays, with certain peak hours consistently showing increased rentals.

When evaluating models, the Random Forest algorithm stood out for its exceptional performance, achieving the lowest RMSLE score.

In summary, our work involved refining data, uncovering trends, selecting the best model, and leveraging predictions. This process has equipped us with actionable insights for informed decision-making.
