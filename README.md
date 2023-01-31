## Project definition:
Finding the perfect restaurant to dine at can be a challenging task, especially with the overwhelming number of options available. A restaurant recommendation system can simplify this process by providing personalized recommendations based on a customer's preferences and past experiences. Our project focuses on developing such a system that utilizes two different algorithms, ALS and Cosine similarity, to provide the most relevant recommendations to its users.

## Model design:


## Research questions:
- Study and develop a restaurant recommendation system that provides personalized recommendations to users in the city of Montreal.
- Research and compare different recommendation system models to determine the best approach for the project.


## Algorithms:
The restaurant recommendation system utilizes two different algorithms, ALS and Cosine similarity, to generate recommendations. The ALS algorithm focuses on matrix factorization to generate latent factors that capture the underlying relationships between customers and restaurants. The Cosine similarity algorithm calculates the similarity between the preferences of a customer and the attributes of a restaurant.


## Dataset:
https://www.kaggle.com/datasets/yelp-dataset/yelp-dataset

The project utilizes a JSON version of the dataset which contains the following files:
1. business.json: Contains business data including location data, attributes, and categories.
2. review.json: Contains full review text data including the user_id that wrote the review and the business_id the review is written for.
3. user.json: User data including the user's friend mapping and all the metadata associated with the user.
4. checkin.json: Checkins on a business.
5. tip.json: Tips written by a user on a business. Tips are shorter than reviews and tend to convey quick suggestions.

The data of 4171 restaurants in Montreal is used to develop the recommendation system.
