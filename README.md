# Movie Recommendation System

## Overview
This project is a movie recommender system implemented using Python and the scikit-learn library. The system suggests movies similar to a given input movie based on their descriptions and genres. The recommendation is made using cosine similarity between the descriptions of movies, which is computed using the Bag-of-Words model.

## Dataset
The dataset used in this project contains information about various movies, including their titles, overviews, genres, and IDs. The dataset is stored in a CSV file named `dataset.csv`.


Certainly! Below is a sample README file for your movie recommender system project on GitHub:

Movie Recommender System
Overview
This project is a movie recommender system implemented using Python and the scikit-learn library. The system suggests movies similar to a given input movie based on their descriptions and genres. The recommendation is made using cosine similarity between the descriptions of movies, which is computed using the Bag-of-Words model.

Dataset
The dataset used in this project contains information about various movies, including their titles, overviews, genres, and IDs. The dataset is stored in a CSV file named dataset.csv.

Implementation Details
1. Data Preprocessing: The dataset is loaded into a Pandas DataFrame, and basic data exploration is performed to understand its structure and contents. Null values are handled, and irrelevant columns are dropped.
1. Text Vectorization: The movie overviews and genres are combined to create a feature vector for each movie using the CountVectorizer from scikit-learn. This vectorization converts text data into numerical format, which can be used for similarity computation.
3. Similarity Computation: Cosine similarity is calculated between the feature vectors of all movies. Cosine similarity measures the similarity between two non-zero vectors of an inner product space and is often used in recommendation systems.
4. Recommendation Generation: Given a movie title as input, the recommender system finds the index of the input movie in the dataset, calculates its similarity with all other movies, and ranks them based on similarity score. The top 5 most similar movies are recommended.

```
Input: Iron Man
Output:
1. Iron Man 2
2. Iron Man 3
3. Captain America: Civil War
4. The Avengers
5. The Incredible Hulk
```

