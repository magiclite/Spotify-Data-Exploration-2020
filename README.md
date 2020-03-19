## Spotify Data Exploration ##

Using Spotify API and my personal streaming data, I analyzed my daily and monthly Spotify usage behavior and my taste in music (e.g. my favorite genres, artists, and tracks). I used data vizualization packages such as plotly to create interactive charts that highlight some of the findings. 

**Data Extraction & API**

●	I requested my streaming data from Spotify in json files, which includes all of my streaming data from March 2019 to March 2020. 

●	The data about artists and tracks were pulled from the Spotify web API, using a library called "spotipy" (<https://spotipy.readthedocs.io/en/latest/#>).

●	I used Python packages including Pandas, Numpy, and Plotly in order to create data structures and interactive data vizualizations.

**Analysis**
1. The line chart shows the mean number of tracks I listened to throughout the day. As expected, I listened to music the most in early morning (6am-9am), when I was usually working out at the gym.

![alt text](https://github.com/magiclite/Spotify-Data-Exploration/blob/master/images/daily_streaming.png)

2. The second chart is a series of box plots, each of which summarizes the aggregate number of songs I listened to each day, broken down by month. I listened to music the most during last October, mostly because I listened to music during midterm season while studying. 

![alt text](https://github.com/magiclite/Spotify-Data-Exploration/blob/master/images/daily_streaming_month.png)

3. The horizontal bar chart shows the top 20 of my favorite genres. The frequency on the x-axis shows the number of times I listened to each genre per day. The color of each bar represents the number of artists in each genre (i.e. the lighter the color of the bar is, the more artists there are in the genre). I listened to pop rap the most, which includes Childish Gambino, Drake, and Chance the Rapper.

![alt text](https://github.com/magiclite/Spotify-Data-Exploration/blob/master/images/my_favorite_genre.png)

4. The scatter plot shows the relationship between release date and 'popularity' of my top 50 tracks. Popularity was sourced from Spotify API and is a pre-calculated index based on how much I listened to the track and its artist. Popularity index ranges between 0 and 100 with 100 being the most popular. The color of each point represents 'danceability' of each track, which was also pulled from Spotify API. We can see that most of my favorite tracks were released between 2012 and 2020 and has danceability of above 0.7. 

![alt text](https://github.com/magiclite/Spotify-Data-Exploration/blob/master/images/release_date_popularity.png)

5. The radar plot shows the average audio features of my favorite tracks. My favorite tracks tend to have high danceability and energy with low speechiness. 

![alt text](https://github.com/magiclite/Spotify-Data-Exploration/blob/master/images/audio_feat.png)
