Project Summary


For our project, our team will be developing a recommender system - more specifically, an anime recommender since all of our team members enjoy watching anime. In order to create this system we will be using two databases that we found on Kaggle. Based on the information of a user, our system will recommend an anime of the same genre. We were also considering creating a form for users, and adding additional questions/fields such as free time - to not only recommend based on rating and genre, but also recommend based on the number of episodes. For instance, a user who is very busy will be less likely to be recommended an anime with a higher number of episodes. 

Our dataset is retrieved from Kaggle and consists of 2 CSV files. 
with 12,294 unique entries, we have 7 features listed below:

Anime_id: Representing the unique ID of the anime 

Name: representing the title of the anime 

Genre: representing all possible genres that the anime falls into 

Type: representing the type of anime. i.e.: TV, movie, oav 

Episodes: representing the number of episodes in the anime 

Rating: representing the average rating of the anime 

Community: Number of community members that are in this anime group 

For our second dataset we have 7,813,737 entries and 3 features listed below: 

user_id: representing the unique ID of the user 

anime_id: representing the unique ID of the anime rated 

rating: representing the rating provided by the user. It ranges from 0 (lowest rating) to 10 (Highest rating). 

For the purposes of this project, we will retain anime_id, name, genre, episodes and rating from the first dataset and all the features from the second dataset. After merging the two tables on anime_id, we had our final dataset of 7 features. Those features will be used in the recommendation process. 

For this recommender system the two algorithms we will be using are Random Forest and Clustering algorithms. Random Forest is a machine learning algorithm. It works by combining the output of many decision trees to reach one single result. This algorithm is good for handling classification problems which is why we chose it as our first algorithm. Our second algorithm is Clustering. Clustering is also a machine learning algorithm that uses unsupervised learning. It groups data into multiple different clusters that contain similar data points. 
For our project, the anime will be clustered based on their genre.



Our machine learning model will consist of a mix of matrix factorization and neural network based model to predict the top 10 animes that match a user profile. Matrix factorization will help us uncover all possible correlations. Neural networks on the other hand have proven themselves to be very efficient in handling multiples features. Due to their structure, neural network based models will help us analyze deeper and extract a robust recommendation.  


