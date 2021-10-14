# The Watcher

Content Based Recommender System recommends movies similar to the movie user likes and analyses the sentiments on the reviews given by the user for that movie.



Check out the live demo: https://the-watcher-s.herokuapp.com/

The details of the movies(title, genre, runtime, rating, poster, etc) are fetched using an API by TMDB, https://www.themoviedb.org/documentation/api, and using the IMDB id of the movie in the API, I did web scraping to get the reviews given by the user in the IMDB site using `beautifulsoup4` and performed sentiment analysis on those reviews.

## How to get the API key?

Create an account in https://www.themoviedb.org/, click on the `API` link from the left hand sidebar in your account settings and fill all the details to apply for API key. You will see the API key in your `API` sidebar once your request is approved.

## Similarity Score : 

   How does it decide which item is most similar to the item user likes? Here we use the similarity scores.
   
   It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.
   
## Evaluation Metric
  Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.
  
  ![image](https://user-images.githubusercontent.com/36665975/70401457-a7530680-1a55-11ea-9158-97d4e8515ca4.png)

  
More about Cosine Similarity : [Understanding the Math behind Cosine Similarity](https://www.machinelearningplus.com/nlp/cosine-similarity/)

### Sources of the datasets 

1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)

### Screenshots

![Screenshot (6)](https://user-images.githubusercontent.com/68689406/137302502-75d54e2f-536b-42f9-85df-60c9e923f980.png)<br>
![Screenshot (9)](https://user-images.githubusercontent.com/68689406/137302587-2f8a2c6c-9760-493e-8af5-31603603cba9.png)<br>
![Screenshot (10)](https://user-images.githubusercontent.com/68689406/137302610-4e9dc1c3-9f69-4150-a3f7-2e612db67aec.png)<br>
![Screenshot (11)](https://user-images.githubusercontent.com/68689406/137303156-ea2c5cf5-2e00-47f5-aed9-336bce980e09.png)<br>



### Methodology/Flowchart
![3](https://user-images.githubusercontent.com/68689406/137303039-1d7a6046-e819-4e63-bd56-d6e4dbe4e507.png)

### Novelty
- Today we are living in a generation that we depend a lot on website based applications, there is a huge amount of information available. We may also get lost in the massive amount of information available in the applications and end up wasting a lot of time in only just trying to find something which we may enjoy watching. The problem is called information overloading problem.<br>

- MOVIE Recommender System (MRS) suggests unseen movies that the user may enjoy, and help them in decision making. MRS helps the applications to perform better and attract users to make the applications successful which makes the RS novel.

- We propose a new strategy for recommender systems evaluation by posing the concept “content novelty”. We define content novelty as the level of novelty of a list of items with respect to the contents. Content novelty combines the best of novelty and diversity approaches in a single and coherent evaluation framework, bridging the gap between both.



