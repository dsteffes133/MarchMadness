This repository contains my work in the Kaggle March Madness Competition. 

The real meat of the work is in the feature engineering.

The first piece of feature engineering was the creation of the ELO variable. ELO was calculated similar to the chess method, by adding or substracting points from the preexisting ELO, based on result and strength of opposition.

Additionally I created derivatives for my features and a rolling window in order to track the momentum of each team and their statistics over the course of the season, and as they approached the tournament.

I then instantiated a random forest regression, an ensemble model that utilizes a "forest" of tree-based models to determine the probability of one team or another winning each respective game.

I separated into train and test sets based on season, and then examined the brier score of my model which is how the model was tested by Kaggle on the new data.
