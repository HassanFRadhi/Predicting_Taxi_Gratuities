# Predicting Taxi Gratuities in New York City

## Overview

The goal of this project was to build a machine learning model to predict whether a taxi rider would leave a high tip or not. The project used yellow taxi trip data from New York City during 2017.
The final random forest model achieved 70.4% accuracy and 74.5% f1-score in identifying generous tippers (more than 20%). Based on the model,  vendor id, mean distance, predicted fare, pickup location - especially location 138 - and mean duration. were the most important factors in distinguishing generous tippers from non-generous tippers (less than 20%).

## Business Understanding

New York City TLC is an agency responsible for licensing and regulating New York City's taxi cabs and for-hire vehicles. The agency has partnered with Automatidata to develop a regression model that helps estimate taxi fares before the ride, based on data that TLC has gathered. 
For this reason, the main business problem of this project was to identify the factors that are most associated with generous tipping behavior.

## Data Understanding

The data used in this project came from the [NYC Taxi and Limousine Commission](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page).
The dataset contained approximately 408,000 taxi trips and 18 features for each trip. These features included information such as trip duration, trip distance, destination, vendor, tolls, payment type, and fare amount.
A new feature was also created to identify whether a trip took place during rush hour or not. Several redundant columns were removed, and the remaining data was converted into the appropriate data types to prepare it for modeling.

## Modeling and Evaluation

A random forest model with 15 decision tree was used to identify which features were most important in predicting generous tipping behavior.
The results showed that vendor id, mean distance, and predicted fare amount were the three most important features in distinguishing generous tippers from non-generous tippers. <br> <br>
<img width="600" height="565" alt="image" src="https://github.com/user-attachments/assets/0b958d19-218d-4264-a4fa-e993e5176ff7" />

The final model achieved:

- 70.4% accuracy
- 74.5% f1-score

These results show that the model was reasonably effective at predicting whether a rider would leave a generous tip.

## Conclusion
This project showed that trip-related factors such as vendor id, mean distance, and predicted fare amount have an important relationship with tipping behavior.
The model can help provide taxi drivers with a better understanding of the factors associated with generous tips. The model should be put into trial so that it can be more tuned and get clear feedback.
Adding more information about a customer behavior with their final tip could also improve the model and provide more useful insights for addressing the business problem.
