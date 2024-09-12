# User-Profiling-and-Content-Recommendation
In the next repository we implement a content-based recommender, a collaborative filtering and a ensemble ti recommend films from an existing database. In this project, we aim to reinforce the concepts behind Audiovisual Recommender Systems. 

## Dataset Exploration and Function Implementations
The entire content of the database has been structured into 3 different dataframes. With Altair's visualization tool, we make a previous analysis about each of the datasets. 

We create various functions, _cardinality_ for example retrieves the number of rows holding the same condition. The _histogram_ function shows the distribution of values for a chosen feature in a dataframe, using a bar plot format. The function _similarity_ calculates the similarity between two vectors, using either the Cosine or Pearson correlation metric. The function _neighbors_ returns the "k" most similar vectors from a matrix given a specific vector. It internally performs a similarity check using the specified metric, either Cosine or Pearson. 

## Content-based filtering
A content-based recommender is implemented and it retrieves the most similar movies based on genre. It generates where, for each movie in the "movies" dataframes 5 recommended movies are provided. We provide 5 recommendations based on the nearest neighbors derived from a feature matrix. The term "feature matrix" in this context refers to he binary genre matrix. 

## Collaborative filtering
A collaborative recommender system prioritizes user preferences over content descriptions. The "ratings" dataframe will be used. We offer 5 recommendations to user based on their provided ratings. We employ the one-hot encoding method. 

## Ensemble filtering
An ensemble recommender combines multiple recommendation algorithms to enhance recommendation accuracy and provide more personalized suggestion, improving user experience and satisfaction.
