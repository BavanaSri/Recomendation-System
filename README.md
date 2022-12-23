# Recomendation-System

Problem Statement: Netflix has a vast users watching different movies from different genres. Provide an algorithm to recommend movies based on watch history

Objective: To recommend movies to Netflix users based on their watch history

Dataset Info: <class 'pandas.core.frame.DataFrame'>
RangeIndex: 1048574 entries, 0 to 1048573
Data columns (total 5 columns):
 #   **Column     Non-Null Count    Dtype** 
---  ------           --------------         ----- 
 0   Cust_Id       1048574 non-null   int64 
 1   Rating        1048574 non-null   int64 
 2   Movie_Id    1048574 non-null   int64 
 3   Genre         1047488 non-null   [object]
 4   MovieName1048574 non-null  object



Data Cleaning:
Null values were observed in genre column. Rows with null values were dropped.

Model Building:

- 1. create a rating matrix for the 'ratings' dataset
- 2. install the scikit-surprise library for implementing SVD
- 3. Load Reader library & Load ratings dataset with Dataset library
- 4. Use the SVD algorithm.
- 5. find all the movies rated as more than 4 stars by user with userId = 1
- 6. Create a shallow copy for the movies dataset
- 7. Reset the index for user_5 dataset
- 8. getting full dataset from Suprise Library
- 9. create a training set for svd
- 10. Predict the ratings for user1
- 11.Drop extra columns from the user1 data frame
- 12. Sort predicted ratings for user1 in descending order
- 13. Print top 10 [recommendations[]
