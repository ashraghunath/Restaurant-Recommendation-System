## Project definition:
Finding the perfect restaurant to dine at can be a challenging task, especially with the overwhelming number of options available. A restaurant recommendation system can simplify this process by providing personalized recommendations based on a customer's preferences and past experiences. Our project focuses on developing such a system that utilizes two different algorithms, ALS and Cosine similarity, to provide the most relevant recommendations to its users.

## Model design:
Restaurant Data model consists of five csv files such as business, checkin, review, tip and user.
business.json : The data represents information about a business including its location, attributes, and categories. It includes details such as the business's address, city, state, and postal code, as well as attributes such as acceptance of credit cards, parking availability, and operating hours. Additionally, the data provides information about the business's geographical location and its rating based on customer reviews. here are 14 features in total, including both numerical and categorical information, as well as dictionary data.
checkin.json : The data represents a list of check-ins at a business, including the dates and times of each check-in.
review.json : This data contains a review of a business, including information such as the reviewer's user ID, the business's ID, the rating given in stars, the number of "useful," "funny," and "cool" votes the review received, the text of the review, and the date the review was written.
tip.json : A tip written by a user on a business is a brief piece of advice or suggestion. It contains information such as the user_id of the person who wrote the tip, the business_id the tip is for, the text of the tip, the date it was written, and the number of compliments received. Tips are typically shorter and more concise than reviews.
user.json : A user profile in a review system typically includes information such as the user's unique identifier, name, number of reviews they've written, the date they started using the system, and their ratings for "useful", "funny", and "cool". It may also include information such as their status as an "elite" user, the number of friends they have on the platform, the number of users who have marked them as a "fan", and their average star rating.
        


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
