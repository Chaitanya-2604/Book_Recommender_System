# Project to build Book_Recommender_System
This project is to build a book recommendation system using the Book Recommendation Dataset. The dataset is available on Kaggle.

# Data

The dataset is available on Kaggle. The dataset contains 3 CSV files. The files are as follows: 

* Books.csv : Contain books details
* Ratings.csv : Contain ratings given by users
* Users.csv : Contain user details
* Dataset columns:
  * Books.csv: ISBN,bookTitle,bookAuthor,yearOfPublication,publisher,Image-URL
  * Ratings.csv: userID,ISBN,bookRating
  * Users.csv: userID, location, age

# Recommendation System

A recommender system, or a recommendation system, is a subclass of information filtering system that seeks to predict the "rating" or "preference" a user would give to an item. They are primarily used in commercial applications. (source - Wikipedia)

Mainly three types of recommendation systems in machine learning based on filtering are used to suggest product and services to the consumers.

* Content Filtering

* Collaborative Filtering

* Hybrid Filtering


* Content Filtering:
  In this algorithm, we try finding items look alike. Once we have item look like matrix,we can easily recommend alike items to a customer, who has         purchased any item from the store.

* Collaborative Filtering:
  Here, we try to search for look alike customers and offer products based on what his/her lookalike has chosen.This algorithm is very effective but takes   a lot of time and resources.

* Hybrid Filtering (Content Filtering + Collaborative Filtering):
  Both Content Filtering & Collaborative Filtering is used for the purpose. you-tube uses this algorithm for their strong recommendation system.
  
  
# Data Cleaning

* The dataset contains less missing values. The missing values samples we dropped from dataset
* Ratings.csv: Contains ratings given by users. Here we are removing the rows which are having rating 0. This is because the rating 0 is not given by the       user. It is given by the system to indicate that the user has not rated the book. So we are removing the rows which are having rating 0.
* Then for each book we are calculating the average rating and the number of ratings. We are also calculating the number of ratings for each user. We are       also calculating the average rating for each user.
* To get a stronger similarity between the books, we are removing the books which are having less than 50 ratings and the users who are having less than 50     ratings.
* Generating the unique books and ISBNs list.



# References 

* Book Recommendation Dataset
* python
* Flask
* Cosine Similarity
* Recommendation System
* seaborn
 
 
 
![recsys_taxonomy2](https://github.com/Chaitanya-2604/Book_Recommender_System/assets/119853009/697624fd-dad8-4cca-b6f4-ea90e37ed909)

