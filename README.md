# Netflix's Recommendation System
#### Co Created by [Ayush Jain](https://www.linkedin.com/in/ayush-jain-290b5a141/), Dhongari Pavan Raj Varma, Nadeeha A, Sreenivasan K V, Romaly Das and Yash Patil
<b> Links: </b> [Collab](https://github.com/ishu1995/NetflixDataset_Clustering/blob/main/TEAM_REALITY_NETFLIX_MOVIES_AND_TV_SHOWS_CLUSTERING.ipynb), [Dataset](https://drive.google.com/file/d/190wMzj1ANCRKxN-oK9w7bPvDPUzQqNVn/view?usp=sharing), [Presentation](https://docs.google.com/presentation/d/14OsZnN7pMv4N2w00e8w_IGXapq4bXF9P/), [Techincal Documentation](https://docs.google.com/document/d/1ZH62x-q-tblzsBx5_1WcX6se0osIqUDI/edit?usp=sharing&ouid=115811449159523075548&rtpof=true&sd=true)
<h3> Business Problem </h3>
Netflix is all about connecting people with their favorite movies. To help customers find preferred movies, they have developed a world-class movie recommendation system: CinematchSM. Their job is to predict whether a person will enjoy a movie based on how much they liked or disliked other movies. Netflix uses those predictions to make recommendations for your movies based on the individual preferences of each customer. And while Cinematch works well, it can always be improved. Now there are so many interesting ways on how Cinematch works that netflix has not tried. Some are described in books, some are not. 

<h3> Problem Statement </h3> 
In 2018, Netflix released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset. Things to do using the dataset: 

1. Exploratory Data Analysis
2. Understanding what type content is available in different countries
3. Is Netflix has increasingly focusing on TV rather than movies in recent years.
4. Clustering similar content by matching text-based features

<b> Tags: Exploratory Data Analysis, Feature Engineering, Machine Learning, Clustering, NLP </b> 

<h3> Available Dataset: </h3>
The dataset consists of  eleven  textual columns and one numeric column.

1. Show id:- It is unique for all the movies/tv shows.
2. Type :- Type of content i.e movie/tv show.
3. Title :- Name of the movie/tv show.
4. Director :- Name of the director
5. Cast:- Actors involved in the movie/tv show.
6. Country :- Country where the movie/tv show is produced.
7. Data added :- Date when movie/tv show is added to Netflix.
8. Release year :- Year when the movie was released.
9. Rating :- Content rating.
10. Listed_in :- Genres of the movie/tv show.
11. Description :- The summary of the movie/tv show.
12. Duration :- total duration of movie in minutes/ seasons for tv shows.

## Approach towards project 
We start our project by doing Data Cleaning and then worked on the basic EDA in which we include: 

1. Compare how many movies and TV Series released on the platform and with the percentage. 
2. Plotting word cloud for more frequent words used in the Title while releasing the content. 
3. Checking the top directors and cast producing content on Netflix 
4. What percentage of content is releasing on Netflix under which segment like Mature Content, Above 17 content etc. 
5. What duration of movies are releasing on the Netflix. 
6. Genre across different countries. 


After basic EDA we tries to figure out what type of content is available in different countries: 

1. We plot country wise grpahs and word clouds to check what type of genre Is releasing in which country. 
2. We also check the content rating for those top genre in all the countries.
3. Country wise word clouds for cast, directors and Title. 


The next step is to figure out if increasingly focus on TV series rather than Movies in recent years. For this we plot a graph in which we show the year wise content added for both TV series and movies. And from that we analyse, In the recent years the rate of producing TV series is clearly high as compared to the Movies.

Now it’s the time to cluster the textual columns to match similar content. For that, we preprocess the textual features using Cleaning, Stopwords, Tokenization, Stemming. Once we got the filtered words we applied vectorization using TD – IDF vectorizer and then applied PCA for dimensionality reduction. 

The prepared text columns were clustered after selecting an optimal value from elbow plots. Finally, we used K Means to cluster our dataset into 9 distinct clusters and we were also able to encode or label the dataset accordingly.

We plot the word clouds of every cluster to check the content we match. 

<b> References: [Deep dive into Netflix's Recommendation System](https://towardsdatascience.com/deep-dive-into-netflixs-recommender-system-341806ae3b48), [Content based recommendation system](https://www.offerzen.com/blog/how-to-build-a-content-based-recommender-system-for-your-product)</b>
