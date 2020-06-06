# Capstone_Project
My Capstone Project for The Data Incubator

As my capstone project for TDI, I build a injury predictor model, aiming to predict the likelihood of an injury among soccer players based on their recent performance data.

Data was scraped from Fbref.com and Transfermarkt, two different online databases of soccer data.
From Transfermarkt we scraped details about the injuries suffered by the players.
From Fbref.com we scraped data regarding the performances of the players in the official matches they played.

We considered matches played in the top 5 European Leagues in the 2017/18 season.

After cleaning the data and assembling it in a proper form, we explored the resulting dataset and experimented with several ML models.
We have an imbalanced classification problem, since the observations resulting in an injury are much fewer than those resulting in no injury.
Using some data augmentation techniques, we trained on a Random Forest Classifier which is (for now) the best performing model.

A Flask app allowing one to experiment by entering the performance data of a player and getting back from the model the likelihood of an injury, is available at https://ronchetti-capstone.herokuapp.com/index_player
