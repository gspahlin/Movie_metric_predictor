# Movie_score_predictor
Can user score be predicted by basic data?

The goal of this project is to be able to predict the success of a movie using data that would be easily obtainable prior to its release. The idea for this project
is similar to the movie analysis I did as a group project during the MSU Data Analytics Bootcamp. In this case I am using machine learning to help me make predictions,
though.

I started with data that my group and I obtained from Kaggle and cleaned in the movie project (https://github.com/gspahlin/Movie_analysis). I have decided to approach 
this as a classification problem to begin with, so I have created a new variable is_liked which corresponds to a user score greater than 6. Most of the features I'm using
are engineered from genre, language and country categories. These columns all contain lists of categorical designations, and I have unpacked them into columns with binary
designations to denote whether certian genres, languages and countries are present in the movie. As of this writing I've implemented a support vector machine model to 
predict whether movies in the test set would be liked. The initial results are encouragning (around 70% accuracy). 

Files:

Movie_predictor.ipynb  - This notebook is where I hammered out my first data set for machine learning application. 

Movie_predictor_ML_1.ipynb  - this is where I have begun implementing machine learning models

IMDb_finalized.csv  - clean dataset from https://github.com/gspahlin/Movie_analysis

ML_dataset1.csv  - dataset created for machine learning application
