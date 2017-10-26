In this project, you'll be working with Jupyter notebook, and analyzing data on movie review scores. 

The dataset is stored in the fandango_score_comparison.csv file. 
It contains information on how major movie review services rated movies. 
The data originally came from FiveThirtyEight.

Here are the first few rows of the data, in CSV format:

FILM	RottenTomatoes	Metacritic	IMDB	Fandango_Stars	RT_norm	RT_user_norm	Fandango_votes
0	Avengers: Age of Ultron (2015)	74	86	7.1	7.8	4.5	3.70	271107
1	Cinderella (2015)	85	80	7.5	7.1	4.5	4.25	65709
2	Ant-Man (2015)	80	90	8.1	7.8	4.5	4.00	103660
3	Do You Believe? (2015)	18	84	4.7	5.4	4.5	0.90	3136
4	Hot Tub Time Machine 2 (2015)	14	28	3.4	5.1	3.0	0.70	19560
Each row represents a single movie. Each column contains information about how the online moview review services RottenTomatoes, Metacritic, IMDB, and Fandango rated the movie. The dataset was put together to help detect bias in the movie review sites. Each of these sites has 2 types of score -- User scores, which aggregate user reviews, and Critic score, which aggregate professional critical reviews of the movie. Each service puts their ratings on a different scale:

RottenTomatoes - 0-100, in increments of 1.
Metacritic - 0-100, in increments of 1.
IMDB - 0-10, in increments of .1.
Fandango - 0-5, in increments of .5.
Typically, the primary score shown by the sites will be the Critic score. Here are descriptions of some of the relevant columns in the dataset:

FILM -- the name of the movie.
RottenTomatoes -- the RottenTomatoes (RT) critic score.
RottenTomatoes_User -- the RT user score.
Metacritic -- the Metacritic critic score.
Metacritic_User -- the Metacritic user score.
IMDB -- the IMDB score given to the movie.
Fandango_Stars -- the number of stars Fandango gave the movie.
To make it easier to compare scores across services, the columns were normalized so their scale and rounding matched the Fandango ratings. Any column with the suffix _norm is the corresponding column changed to a 0-5 scale. For example, RT_norm takes the RottenTomatoes column and turns it into a 0-5 scale from a 0-100 scale. Any column with the suffix _round is the rounded version of another column. For example, RT_user_norm_round rounds the RT_user_norm column to the nearest .5.
