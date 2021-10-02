[ProjectSummary_Netflix.docx](https://github.com/ishu1995/NetflixDataset_Clustering/files/7150006/ProjectSummary_Netflix.docx)
# NetflixDataset_Clustering
In our problem statement of Netflix movies and Tv Series Clustering, we have given 4 tasks to execute mention below: 

Exploratory Data Analysis
Understanding what type of content is available in different Countries
Is Netflix has increasingly focused on TV rather than Movies in recent years?
Clustering similar content by matching text based features.

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

In the last, now it’s the time to cluster the textual columns to match similar content. For that, we preprocess the textual features using Cleaning, Stopwords, Tokenization, Stemming. Once we got the filtered words we applied vectorization using TD – IDF vectorizer and then applied PCA for dimensionality reduction. 

Now we figure out the optimal value of K for Clustering through Elbow method and Silhouette method and the number come to 9. 
Once we did the clustering, we got 9 clusters namely: 

0: Kids, Animation & Anime
1: Musical International & Indian
2: Drama, International, Indian
3: Documentaries, Sports
4: Drama, American, Adventure
5: Comedy
6: Horror
7: International TV Shows
8: Family Movies

We plot the word clouds of every cluster to check the content we match. 
