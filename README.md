# pyspark
In this project, I address the business problem of predicting the favorite genres of anime for different age groups.
To accomplish this task, I have gathered data on users' profile information and their favorite anime genres from the datasets, respectively.
I have cleaned and preprocessed the data to remove any inconsistencies and make it ready for analysis.
Next, I have joined the necessary tables to create a new table that provides a comprehensive view of the user's age group and their favorite genres of anime. 
I have used this DataFrame to train and evaluate five different models: Logistic regression, random forests, decision tree, and neural network.
My aim is to identify the model that best predicts the favorite genres of anime for users based on their age group. 
By doing so, I can provide recommendations to streaming services and production companies to cater to their audience's preferences and improve their business performance

# The Dataset:
The dataset was obtained from kaggle.
This dataset contains informations about Anime (16k), Reviews (130k) and Profiles (47k) crawled from https://myanimelist.net/ at 05/01/20.
The crawler program is opened on https://github.com/marlesson/scrapy_myanimelist
There are others similar datasets:
  • azathoth42/myanimelist
  • CooperUnion/anime-recommendations-database
  • natlee/myanimelist-comment-dataset
Content:
The dataset contains 3 files:
  • animes.csv contains list of anime, with title, title synonyms, genre, duration, rank, populatiry, score, airing date,
episodes and many other important data about individual anime providing sufficient information about trends in time about important aspects of anime. 
Rank is in float format in csv, but it contains only integer value. This is due to NaN values and their representation in pandas.
  • profiles.csv contains information about users who watch anime, namely username, birth date, gender, and their favorite animes list.
  • reviews.csv contains information about reviews: users x animes, with text review and scores.
