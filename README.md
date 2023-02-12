## Project definition:
Finding the perfect restaurant to dine at can be a challenging task, especially with the overwhelming number of options available. A restaurant recommendation system can simplify this process by providing personalized recommendations based on a customer's preferences and past experiences. Our project focuses on developing such a system that provides the most relevant recommendations to its users.

## Research questions:
1. Study and develop a restaurant recommendation system that provides personalized recommendations to users in the city of Montreal.
2. Research and compare different recommendation system models to determine the best approach for the project.
3. What are the top similar restaurants based on the reviews given by a user ?
4. Recommend top restaurants based on a specific keyword like, 'Thai', 'Mexican' or 'pizza', 'sandwich' etc.

## Model 1 : Content based recommendation system 
This code implements a Content-based Similarity Recommendation System for restaurants. In a content-based recommendation system, the system suggests items to a user based on their past preferences and behavior, as represented by their interaction with items. In this code, the focus is on suggesting restaurants to a user based on the user's past restaurant reviews.

Algorithm:
The cosine similarity algorithm is used to calculate the similarity between the user's past reviews or the keyword and the restaurant reviews. The user's past reviews are transformed into word vectors using a pre-trained pipeline model and the resulting vectors are used to calculate the cosine similarity between the user's past reviews and the restaurant reviews. The restaurants with the highest cosine similarity scores are considered the most similar to the user's past preferences and are recommended to the user. In the case of keyword-based similarity, the keyword is transformed into a word vector and its cosine similarity with the restaurant reviews is calculated to find the top 10 recommended restaurants based on the keyword.

## Model 2 : Content based recommendation system 
