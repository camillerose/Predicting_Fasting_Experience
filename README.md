# Predicting Fasting Experience
This notebook uses data from a fasting app to predict whether someone will have a positive or negative fasting experience. In addition, there is a heavy exploratory data analysis component in this notebook, including k-means clustering, the labels of which are used in a random forest regression model. This analysis was completed in 8 hours.

## Goals:
- Identify key factors that influence a user’s fasting experience
- Cluster users by engagement level with app and extracts insights about each cluster
- Build a classification model to predict whether a user will have a positive or negative fasting experience

## Approach
1. Explore the data identifying features that are associated with a difference in fasting experience
2. Use K-means clusters and feature engineering to cluster users by app engagement
3. Build and tune a random forest classifier. Use the feature importances to bolster (1).

## Model Result



## Features
fasting_app_users.csv
- user_id: user id
- reason_for_fasting: reason given by user for engaging in fasting
- type_of_fast: type of fast the user is participating in (e.g., 18 hours)
- fasting_notification: time fasting notification is set (if no notification is set, nan)
- age: user age
- gender: user gender


fasting_log.csv
- user_id: user id
- timestamp: time log was made
- fasting_duration: length of fast
- hunger_level: 0-100 (100 being extremely hungry)
- last_meal_count: majority of the content of the last meal before the fast began
- motivations: motivations indicated by user as influencing fasting behavior
- fasting_experience: the outcome of the fast indicated by the user
