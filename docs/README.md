#  Advanced Film Suggestion

## Objective
The objective of this project is to build a robust Movie Recommender System that provides personalized movie recommendations to users. This system is a part of my Springboard Capstone Project on Movie Data Analysis and Recommendation Systems. The project is divided into two parts, with the first part focusing on an extensive exploratory data analysis of movie metadata collected from TMDB, and the second part, detailed in this notebook, focusing on implementing various recommendation algorithms to build an ensemble model for movie recommendations.

## Tools Used
- Python
- Pandas
- Scikit-learn
- Surprise Library
- TMDB API
- MovieLens Datasets

## Concepts Used
- Exploratory Data Analysis (EDA)
- Content-Based Filtering
- Collaborative Filtering
- Singular Value Decomposition (SVD)
- Ensemble Modeling
- Cosine Similarity
- IMDB Weighted Rating System

## Dataset
The project utilizes two datasets from MovieLens:
1. **Full Dataset**: Comprises 26,000,000 ratings and 750,000 tag applications applied to 45,000 movies by 270,000 users. Includes tag genome data with 12 million relevance scores across 1,100 tags.
2. **Small Dataset**: Comprises 100,000 ratings and 1,300 tag applications applied to 9,000 movies by 700 users.

## Methodology
1. **Simple Recommender**: 
   - Provides generalized recommendations based on movie popularity and genre.
   - Utilizes TMDB Ratings and IMDB's weighted rating formula to sort movies based on ratings and popularity.
   
2. **Content-Based Recommender**:
   - Provides personalized recommendations based on movie metadata.
   - Two models were built, one based on movie overviews and taglines, and the other based on movie cast, crew, keywords, and genre.
   
3. **Collaborative Filtering**:
   - Utilizes the Surprise library to build a collaborative filter based on Singular Value Decomposition (SVD).
   - Aims to minimize Root Mean Square Error (RMSE) to provide accurate recommendations.
   
4. **Hybrid Engine**:
   - Combines the Content-Based and Collaborative Filtering approaches to provide personalized movie suggestions based on estimated ratings for a particular user.

## Results
- The Simple Recommender was able to provide generalized recommendations based on movie popularity and genre.
- The Content-Based Recommenders were able to provide more personalized recommendations, with the metadata-based recommender showing more promise due to the inclusion of additional suggestive metadata.
- The Collaborative Filtering approach was able to capture user preferences across different genres and provide personalized recommendations.
- The Hybrid Engine successfully combined the strengths of both Content-Based and Collaborative Filtering approaches to provide more personalized and accurate recommendations.

## Conclusions
The project successfully demonstrates the implementation of various recommendation algorithms to build a robust Movie Recommender System. The Hybrid Engine, combining both content-based and collaborative filtering approaches, shows a promising strategy for providing personalized movie recommendations to users. The project also highlights the importance of using suggestive metadata and powerful algorithms like SVD to improve the accuracy and quality of recommendations.

## Future Work
- Explore other hybrid models and algorithms to further improve the recommendation quality.
- Incorporate additional data such as user profiles and movie attributes to enhance the personalization aspect of the recommender system.
- Optimize the system for scalability to handle larger datasets and ensure real-time recommendations.


