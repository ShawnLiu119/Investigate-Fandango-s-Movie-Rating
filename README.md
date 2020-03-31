# Investigate-Fandango-s-Movie-Rating
Is Fandangoo' rating inflated? 


In October 2015, a data journalist named Walt Hickey analyzed movie ratings data and found strong evidence to suggest that Fandango's rating system was biased and dishonest (Fandango is an online movie ratings aggregator). He published his analysis in this article — a great piece of data journalism that's totally worth reading.
The goal for this project is to determine whether there has been any change in Fandango's rating system after Hickey's analysis

raw data could be downloaded here,
Walt Hickey made the data he analyzed publicly available on GitHub. We'll use the data he collected to analyze the characteristics of Fandango's rating system previous to his analysis.
https://github.com/fivethirtyeight/data/blob/master/fandango/fandango_score_comparison.csv

One of Dataquest's team members collected movie ratings data for movies released in 2016 and 2017. The data is publicly available on GitHub and we'll use it to analyze the rating system's characteristics after Hickey's analysis.
https://github.com/mircealex/Movie_ratings_2016_17


fandango_score_comparison.csv contains every film that has a Rotten Tomatoes rating, a RT User rating, a Metacritic score, a Metacritic User score, and IMDb score, and at least 30 fan reviews on Fandango. The data from Fandango was pulled on Aug. 24, 2015.

Column	Definition
FILM	The film in question
RottenTomatoes	The Rotten Tomatoes Tomatometer score for the film
RottenTomatoes_User	The Rotten Tomatoes user score for the film
Metacritic	The Metacritic critic score for the film
Metacritic_User	The Metacritic user score for the film
IMDB	The IMDb user score for the film
Fandango_Stars	The number of stars the film had on its Fandango movie page
Fandango_Ratingvalue	The Fandango ratingValue for the film, as pulled from the HTML of each page. This is the actual average score the movie obtained.
RT_norm	The Rotten Tomatoes Tomatometer score for the film , normalized to a 0 to 5 point system
RT_user_norm	The Rotten Tomatoes user score for the film , normalized to a 0 to 5 point system
Metacritic_norm	The Metacritic critic score for the film, normalized to a 0 to 5 point system
Metacritic_user_nom	The Metacritic user score for the film, normalized to a 0 to 5 point system
IMDB_norm	The IMDb user score for the film, normalized to a 0 to 5 point system
RT_norm_round	The Rotten Tomatoes Tomatometer score for the film , normalized to a 0 to 5 point system and rounded to the nearest half-star
RT_user_norm_round	The Rotten Tomatoes user score for the film , normalized to a 0 to 5 point system and rounded to the nearest half-star
Metacritic_norm_round	The Metacritic critic score for the film, normalized to a 0 to 5 point system and rounded to the nearest half-star
Metacritic_user_norm_round	The Metacritic user score for the film, normalized to a 0 to 5 point system and rounded to the nearest half-star
IMDB_norm_round	The IMDb user score for the film, normalized to a 0 to 5 point system and rounded to the nearest half-star
Metacritic_user_vote_count	The number of user votes the film had on Metacritic
IMDB_user_vote_count	The number of user votes the film had on IMDb
Fandango_votes	The number of user votes the film had on Fandango
Fandango_Difference	The difference between the presented Fandango_Stars and the actual Fandango_Ratingvalue
