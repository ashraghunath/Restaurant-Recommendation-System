## Project definition:
The goal of our project is to develop a restaurant recommendation system for the city of Montreal which provides personalized recommendations based on customer's reviews and ratings for the restaurant.

## Research questions:
1. Is collaborative-filtering a good model for recommending restaurants? If so, what's the purpose of it?
2. What is the purpose of collaborative-filtering in recommendation systems?

3. Compare content-based and collaborative-filtering to determine the best approach for this project.
4. What are the top similar restaurants based on the previous reviews given by a user ?
5. Recommend top restaurants based on a particular keyword like, 'Italian' or 'Burgers' etc.

## Dataset

The data set contains 8,021,122 reviews on 209,393 businesses in 11 metropolitan areas out of which we have 4,171 restaurants in Montreal.

In this project, business.json, review.json and user.json files will be utilized from the dataset.

* business.json : The data represents information about a business including its location, attributes, and categories. It includes details such as the business's address, city, state, and postal code, as well as attributes such as acceptance of credit cards, parking availability, and operating hours. Additionally, the data provides information about the business's geographical location and its rating based on customer reviews. here are 14 features in total, including both numerical and categorical information, as well as dictionary data.
* review.json : This data contains a review of a business, including information such as the reviewer's user ID, the business's ID, the rating given in stars, the number of "useful," "funny," and "cool" votes the review received, the text of the review, and the date the review was written.
* user.json : The user data includes information such as the user ID, name, number of reviews they've written and the number of times their ratings were "useful", "funny", and "cool". 

Link : https://www.kaggle.com/datasets/yelp-dataset/yelp-dataset

## Model 1 : Content based filtering
This model focuses on suggesting restaurants to a user based on the user's past restaurant reviews along with the keywords provided.

**Algorithm:**
The cosine similarity algorithm is used to calculate the similarity between the user's past reviews or the keyword and the restaurant reviews. The restaurants with the highest cosine similarity scores are considered the most similar to the user's past reviews and are recommended to the user. In the case of keyword-based similarity, the keyword and its cosine similarity with the restaurant reviews is calculated to find the top recommendations.

## Model 2 : Collaborative filtering

In this model, we use collaborative filtering model to recommend restaurants to users based on their ratings compared to that of similar user’s.

**Algorithm:**
We shall use ALS algorithm to make predictions about the ratings that a user might give to a restaurant. The goal of the matrix factorization is to factorize the user-restaurant rating matrix into user-feature and restaurant-feature matrices. These matrices are then used to make predictions about missing ratings in the original matrix.
