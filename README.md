# Books-Recommender-System-Using-Machine-Learning

Given the hectic nature of modern life, recommendation systems are gaining prominence. There are so many things that people have to do in a day that they never have enough time. Since recommendation systems aid users in making correct selections with little mental effort, they are crucial.

In its most basic form, a recommendation system seeks for material that a user would find engaging. In addition, there are a lot of moving parts involved in making unique, user-specific recommendations of relevant and engaging material. An individual may use a recommendation system, which is an algorithm based on artificial intelligence, to quickly scan all of the available possibilities and provide a personalized list of things that are likely to pique their interest. Their profile, search and browsing history, the viewing habits of those who have their characteristics and demographics, and your own likelihood of like those films all go into these recommendations. Heuristics and predictive modeling using the given data do this.

# Types of Recommendation System :

### 1 ) Content Based :
- content-based systems, which think about item attributes and employ identifying information.
- YouTube and Twitter.
- The artist you're viewing and the song you're listening to. Form embeddings for the features .
- The suggestion of user-specific activities or comparable goods.
- It'll make a vector representation of it.
- In order to provide suggestions, these systems analyze the user's profile and the items they own. They postulate that a user's prior interest in an item is indicative of their future interest in it.
- Too much specialization might lead to suggestions that are obviously not relevant to the user; for example, if user A is only interested in categories B, C, and D, the system will not be able to suggest anything outside of those categories, even if those things could be of interest to user A.

### 2 ) Collaborative Based :
- Systems that work together to filter items based on interactions between users and items.
- Groups of people who have similar ratings or characteristics.
- Cluster technique for book suggestion.
- Our only metric is user feedback in the form of ratings or comments.
- Simply put, collaborative filtering systems work on the premise that a user's interest in one item (A) can be indicative of that user's interest in another (B) if both users have shown an affinity for A and B.

- Problems include:
    - Computing the User-Item nXn matrix is computationally costy.
    - We will only recommend well-known goods.
    - In some cases, new products may not be recommended at all.
 
### 3 ) Hybrid Based :
- Hybrid systems, which integrate two forms of data in an effort to sidestep issues that arise when dealing with one kind alone.
- Both are used together nowadays.
- Uses : word2vec , embedding . 

# About this project:
This is a collaborative filtering based books recommender system & a streamlit web application that can recommend various kinds of similar books based on user interest.

# Demo:

<img src="templates/1.png" alt="workflow" width="70%">

<img src="templates/2.png" alt="workflow" width="70%">

# Concept used to build the model.pkl file : NearestNeighbors

1 . Load the data
	
2 . Initialise the value of k

3 . For getting the predicted class, iterate from 1 to total number of training data points

4 . Calculate the distance between test data and each row of training data. Here we will use Euclidean distance as our distance metric since it’s the most popular method. 

5 . Sort the calculated distances in ascending order based on distance values
	
6 . Get top k rows from the sorted array

# Built With
1. streamlit
2. Machine learning
3. sklearn

## Heroku Commands
$ heroku login -i

$ git init

$ heroku git:remote -a book-recommendation-system13

$ git add . 

$ git commit -am "make it better"

$ git push heroku master


