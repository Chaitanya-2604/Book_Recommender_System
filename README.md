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
