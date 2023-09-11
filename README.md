#### runner_rank_prediction

# Race Ranking Prediction Overview
This project aims to predict race rankings based on various features and attributes related to athletes and their prior race performances. We explore the relationship between ranking and different factors like price, gender, age, previous race history, and race types.

# Code Structure
The project code is organized into several sections:

## Exploratory Data Analysis (EDA):

- Analyzes the relationship between ranking and price.
- Explores the differences in ranking distribution between male and female athletes.
- Investigates the influence of the number of previous races on ranking.
- Examines the impact of different race types on ranking.

## Data Preprocessing:

- Contains custom preprocessing classes for handling and transforming data.
- Includes preprocessing for gender, race distances, the number of previous races, and incomplete races.
- One-hot encodes race types.

## Model Building:

- Utilizes machine learning techniques to predict rankings.
- Applies a Random Forest Regressor and conducts hyperparameter tuning.

## Custom Preprocessing
Several custom preprocessing classes have been defined to handle specific data transformations:

- SexPreprocessor: Standardizes gender values and handles unspecified values.
- DistPreprocessor: Calculates the distance of each race course.
- NumRacesPreprocessor: Counts the number of previous races for each user.
- IncompleteRacesPreprocessor: Determines the number of prior incomplete races per user.
- RaceTypeEncoder: Performs one-hot encoding for race types.

## Hyperparameter Tuning
- Hyperparameter tuning is carried out using RandomizedSearchCV to find the best parameters for the Random Forest Regressor.
