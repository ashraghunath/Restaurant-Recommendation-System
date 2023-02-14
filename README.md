## Project definition:
Finding the perfect restaurant to dine at can be a challenging task, especially with the overwhelming number of options available. A restaurant recommendation system can simplify this process by providing personalized recommendations based on a customer's preferences and past experiences. Our project focuses on developing such a system that provides the most relevant recommendations to its users.

## Research questions:
1. Study and develop a restaurant recommendation system that provides personalized recommendations to users in the city of Montreal.
2. Which model among content-based and collborative-filtering method is better for recommending restaurants?
3. What are the top similar restaurants based on the reviews given by a user ?
4. Recommend top restaurants based on a specific keyword like, 'Thai', 'Mexican' or 'pizza', 'sandwich' etc.

## Dataset

The data set contains 8021122 reviews on 209393 businesses in 11 metropolitan areas out of which we have 8679 restaurants in Toronto and 4171 in Montreal.

In this project, business.json, review.json and user.json files will be utilized from the dataset.

* business.json : The data represents information about a business including its location, attributes, and categories. It includes details such as the business's address, city, state, and postal code, as well as attributes such as acceptance of credit cards, parking availability, and operating hours. Additionally, the data provides information about the business's geographical location and its rating based on customer reviews. here are 14 features in total, including both numerical and categorical information, as well as dictionary data.
* review.json : This data contains a review of a business, including information such as the reviewer's user ID, the business's ID, the rating given in stars, the number of "useful," "funny," and "cool" votes the review received, the text of the review, and the date the review was written.
* user.json : A user profile in a review system typically includes information such as the user's unique identifier, name, number of reviews they've written, the date they started using the system, and their ratings for "useful", "funny", and "cool". It may also include information such as their status as an "elite" user, the number of friends they have on the platform, the number of users who have marked them as a "fan", and their average star rating.

Link : https://www.kaggle.com/datasets/yelp-dataset/yelp-dataset

## Model 1 : Content based 
This code implements a Content-based Similarity Recommendation System for restaurants. In a content-based recommendation system, the system suggests items to a user based on their past preferences and behavior, as represented by their interaction with items. In this code, the focus is on suggesting restaurants to a user based on the user's past restaurant reviews.

**Algorithm:**
The cosine similarity algorithm is used to calculate the similarity between the user's past reviews or the keyword and the restaurant reviews. The user's past reviews are transformed into word vectors using a pre-trained pipeline model and the resulting vectors are used to calculate the cosine similarity between the user's past reviews and the restaurant reviews. The restaurants with the highest cosine similarity scores are considered the most similar to the user's past preferences and are recommended to the user. In the case of keyword-based similarity, the keyword is transformed into a word vector and its cosine similarity with the restaurant reviews is calculated to find the top 10 recommended restaurants based on the keyword.

## Model 2 : Collaborative filtering

In the code, the ALS algorithm is used to recommend restaurants to users based on their ratings compared to similar user’s.

Algorithm:

ALS algorithm to make predictions about the ratings that a user might give to a restaurant. 
The goal of the matrix factorization is to factorize the user-restaurant rating matrix (sparse matrix) 
into product of two low dimensional user-feature and restaurant-feature matrices which will allow model
to recommend better personalized restaurants to users. These matrices are then used to make predictions 
about missing ratings in the original matrix. Matrix factorization is one of the very effective 
dimensionality reduction technique in machine learning. 
