# Movie Recommender Project

### Premise

There are so many movies out there to watch and there are a lot of venues to watch those movies especially with all the streaming services out there. No one likes to sit there for too long trying to figure out what they want to watch. Switching between streaming services and continually scrolling trying to figure out what sounds good. Some people will even seek out the advice of their one friend that they deem the “movie person” and ask for recommendations to watch. As a service to their subscribers, many streaming services are using recommender systems to aid in the task of finding something interesting to watch. The services will recommend a movie to watch based on the movie that the subscriber just finished watching or based on the subscriber’s viewing history. For this project, datasets from the International Movie Database, or IMDb, will be used to develop a movie recommender system.

### Problem Statement

<div align = 'center'>Using the IMDb datasets, can a movie recommendation system be built based on a given movie title?</div>

### Methods              
              
The data for this project comes from https://m.imdb.com/interfaces/, and was downloaded on October 27, 2021.
  
  The first recommender that was made is a content-based recommender based on genre of the title. To do this, we will use the concepts of vectors and their proximity to each other to make recommendations. We must first transform the genres into a vector through TFID-Vectorization and the use the cosine similarity to determine the recommendations. However, as this model was being built, there was an issue with the size of the dataset, so it was subset further by the year of the movie and the tvshows and tvmovies were dropped and this left 21,053 titles.
  
  The second recommender used both the subset dataset first and then used the full dataset to make recommendations. The second recommender used the concept of nearest neighbor to provide recommendations. A pivot table was created using the title, genre and average rating. That was then put into a matrix and the cosine similarity is used again to find the other titles that are closest to the title.
              
              
