# Movie Recommendation System using Collaborative Filtering 

Collaborative filtering predicts user preferences by analyzing patterns of behavior across users and items. It uses a matrix to map user interactions, such as movie ratings, and plots these as data points in a vector space. Similarity between users or items is then measured by calculating the distances between these points.

The process begins with data preprocessing, which involves loading the datasets of movies and user ratings. Once the data is loaded, the movie and rating datasets are combined based on a common identifier, such as movieID. To ensure the quality of recommendations, movies that have been rated by fewer than 10 users are removed from the dataset. This filtering step helps to focus on items with sufficient user interaction, thereby enhancing the reliability of the similarity calculations. Additionally, the rating values are normalized on a row-wise basis, ensuring that the ratings are adjusted relative to each user's overall rating behavior.

A similarity matrix is created based on the normalized ratings. The system calculates a personalized similarity score for each movie by adjusting precomputed scores according to the user's specific rating. This generates an array of similarity scores, helping identify movies that match the user’s preferences.

The similarity scores are aggregated to produce personalized recommendations. For each rated movie, similarity scores with other movies are calculated, summed, and sorted to highlight the top recommendations. The result is a set of movies most aligned with the user's tastes.
