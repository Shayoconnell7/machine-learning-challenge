# machine-learning-challenge

## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, I have created several machine learning models capable of classifying candidate exoplanets from the raw dataset.


## Process

- For all models, the initial processes were the same:
        I cleaned the data some, selected features, split the data into train and test sections, and scaled the values for X. Depending on the model, I sometimes encoded the y data.
- Initially, I used all features to create a basic version of each of the following model types (notebooks named as such):
        logistic_regression_model( 0.8443935926773455), linear_regression_model(.4756191826064569), k_nearest_neighbor_model(0.823), decision_trees_model (accuracy: 0.8489702517162472), random_forest_model(0.8861556053161621), neural_network_model(0.8861556053161621), deep_neural_network_model(0.8850114345550537)
- I then compared the accuracy of each model, and found the most accurate one to be the random_forest_model and neural_network_model
- I chose to continue with only the random_forest_model, and created random_forest_model_-_2 for feature selection, which allowed me to raise the accuracy slightly.
- I then used GridSearch on random_forest_model_2 to hypertune the parameters
- This resulted in a final model with an accuracy score of 
- I saved this model
