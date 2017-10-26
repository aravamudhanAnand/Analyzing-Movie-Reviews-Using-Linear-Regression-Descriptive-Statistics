In this project, you'll be working with Jupyter notebook, and analyzing data on movie review scores. 

The dataset is stored in the fandango_score_comparison.csv file. 
It contains information on how major movie review services rated movies. 
The data originally came from FiveThirtyEight.

Each row represents a single movie. Each column contains information about how the online moview review services RottenTomatoes, Metacritic, IMDB, and Fandango rated the movie. The dataset was put together to help detect bias in the movie review sites. Each of these sites has 2 types of score -- User scores, which aggregate user reviews, and Critic score, which aggregate professional critical reviews of the movie. Each service puts their ratings on a different scale:

RottenTomatoes - 0-100, in increments of 1.
Metacritic - 0-100, in increments of 1.
IMDB - 0-10, in increments of .1.
Fandango - 0-5, in increments of .5.
Typically, the primary score shown by the sites will be the Critic score. 

Here are descriptions of some of the relevant columns in the dataset:

FILM -- the name of the movie.
RottenTomatoes -- the RottenTomatoes (RT) critic score.
RottenTomatoes_User -- the RT user score.
Metacritic -- the Metacritic critic score.
Metacritic_User -- the Metacritic user score.
IMDB -- the IMDB score given to the movie.
Fandango_Stars -- the number of stars Fandango gave the movie.

