# Elastic-Net-For-Car-Price-Prediction

In this github repository we describe our project which contains three parts

#1. Web Scraping
We web scrape data from an online website that puts up different items for sale, we specifically extract data for cars using beautiful soup library.
We then sort the data into a pandas data frame with 19 columns and we sort the data in a manner that will then be suitable for training a model in order to predict the car's price.
We also scrape data using an API from a public website in order to build a supply score that will further more help us in predicting the price.

#2. Preparing the data and training the model
We create a function prepare_data where we prepare the data for input into the Elastic Net model for predicting price of car.
We then create a pipeline in order to make sure all the data goes under the same precedure in training and to avoid data leakage.
We use gridsearch in order to optimize the model's hyper parameters and get the best result.
We end up with an RMSE of 9880.

#3. Flask Application
We create a flask application in order to make the trained model available for easier use.
We create an index.html page where we aquire the user to input relevant information which the model will use to predict the price.

# Summary
In this project we used web scraping techniques in order to get data from different sources in an efficient manner. 
We then take the data and prepare it for training and train an Elastic Net Regression model. 
We then create Flask Application in order to make the use of the model easier.
