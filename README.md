# Recommender-System

## Handling Item Cold Start Problem in Recommender Systems using Text and Visual Embeddings.

The proposed method for our hybrid movie recommendation can be divided into four parts.
The inputs available are user-movie ratings, movie genre, movie plots, and movie trailers. Second, we create movie vectors using plot vectors and trailer vectors. For plot vectors, we
use sentence embeddings of the plot of the movie using SBERT. We use the ResNet-BiLSTM model for trailer vectors to represent trailer features in terms of movie genre probabilities.
Subsequently, we generate user-profile vectors using a Deep Neural Network. These user profile vectors work to capture the hidden interests of the user and are made up of vectors
of movies that are liked(rating above a threshold) by the user. Capturing the interests and tastes of the user is necessary for the personalization of recommendations and helps solve
the item cold-start problem. Finally, deciding whether to recommend a movie or not to a user and generating top-N recommendations are described.

# Proposed Architecture Diagram:
![Proposed Arch Diag](https://github.com/babyitachi/Recommender-System/blob/master/visuals/Arch%20diag%20with%20bg.png)
