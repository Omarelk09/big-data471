# big-data471

Project Summary
Instructions:
Project summary (10%) The project summary will be a 400-word abstract available as a Markdown (.md) document in a GitHub repository. The summary will report on project definition and model design. It will describe the dataset and its main characteristics (number and type of features), the research questions to be addressed in the project, the class of models to be applied to the dataset, and the algorithms that will be used. At least two algorithms must be used and compared. The project summary will be evaluated during the project clinics

For our project, our team will be developing a recommender system - more specifically, an anime recommender since all of our team members enjoy watching anime. In order to create this system we will be using two databases that we found on Kaggle. Based on the information of a user, our system will recommend an anime of the same genre. We were also considering creating a form for users, and adding additional questions/fields such as free time - to not only recommend based on rating and genre, but also recommend based on the number of episodes. For instance, a user who is very busy will be less likely to be recommended an anime with a higher number of episodes. 

Our dataset is retrieved from Kaggle and consists of 2 CSV files. 
The first is an anime database containing 12,294 unique entries, all representing an anime and all its features. In this dataset, we have 7 features listed below: 
Anime_id: Representing the unique ID of the anime (Int)
Name: representing the title of the anime (String)
Genre: representing all possible genres that the anime falls into (String)
Type: representing the type of anime. i.e.: TV, movie, oav (String)
Episodes: representing the number of episodes in the anime (Int)
Rating: representing the average rating of the anime (Double)
Community: Number of community members that are in this anime group (Int)
Next, we are using a second dataset consisting of user ratings. It includes the ratings that users are giving to anime they have watched. It contains 7,813,737 entries and 3 features listed below: 
user_id: representing the unique ID of the user (Int)
anime_id: representing the unique ID of the anime rated (Int)
rating: representing the rating provided by the user. It ranges from 0 (lowest rating) to 10 (Highest rating). Also, the rating is set to ‘-1’ if the user did rate the anime. 

For the purposes of this project, we will retain anime_id, name, genre, episodes and rating from the first dataset and all the features from the second dataset. After merging the two tables on anime_id, we had our final dataset of 7 features. Those features will be used in the recommendation process. 

Our machine learning model will consist of a mix of matrix factorization and neural network based model to predict the top 10 animes that match a user profile. Matrix factorization will help us uncover all possible correlations. Neural networks on the other hand have proven themselves to be very efficient in handling multiples features. Due to their structure, neural network based models will help us analyze deeper and extract a robust recommendation.  
