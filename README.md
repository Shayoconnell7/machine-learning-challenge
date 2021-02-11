# machine-learning-challenge

## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, I have created several machine learning models capable of classifying candidate exoplanets from the raw dataset.


## Process

- For all models, the initial processes were the same:
        I cleaned the data some, selected features, split the data into train and test sections, and scaled the values for X. Depending on the model, I sometimes encoded the y data.
- Initially, I used all features to create a basic version of each of the following model types (notebooks named as such):
        logistic_regression_model( 0.8443935926773455), linear_regression_model(.4756191826064569), k_nearest_neighbor_model(0.823), decision_trees_model (accuracy: 0.8489702517162472), random_forest_model(0.8861556053161621), neural_network_model(0.8861556053161621), deep_neural_network_model(0.8850114345550537)
- I then compared the accuracy of each model, and found the most accurate ones to be the random_forest_model and the neural_network_model. However, since the scores for random_forest_model and neural_network_model were identical, and I did not have success attempting GridSearch for the neural_network_model, I chose to continue with random_forest_model and logistic_regression_model, which was another fairly high score.
- I created random_forest_model_2 and logistic_regression_model_2, and did further feature selection for both, based on feature_importances run in my original in the random_forest_model, which allowed me to raise the accuracy slightly.
- I then used GridSearch on each to hypertune the parameters for each.
- This resulted in a final model with an accuracy score of 0.8952854044928286 for random_forest_model_2 and 0.8868937337631623 for logistic_regression_model_2.
- Since the score for random_forest_model_2 was slightly higher, I saved this model.


