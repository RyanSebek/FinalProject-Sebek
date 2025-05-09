# FinalProject-Sebek

# Kmeans Clustering - Spotify Songs
## Abstract
Do you ever get tired of listening to the same songs on repeat? Finding new songs has never been easier with machine learning. By using using the k-nearest neighbor algorithm and KMeans, the computer is able to group songs that share similar characteristics. These models were selected because of how effective they are with larger datasets as well as how they classify songs into groups. These groups that get created are what is used for song recommendations. In order to test the algorithm, a data set containing nearly 200,000 songs will be used. This data set provides the algorithm with numerous variables including release data, tempo and how loud the song is. While these are nice to have, the primary features people look to when listening to music are the genre, the tempo, and the emotion of the song. 

## Introduction
Using Kmeans clustering, I classified songs given a variety of variables such as tempo, dancability, and popularity. This study was conducted using a spotify songs dataset with over 200,000 unique songs. The study utilizes silhouette scores in order to evaluate the effectiveness of the model when applied to the following dataset. 

## Related Work
While working on this study, I referenced a similar work done by Emmanuel Katwebaze. In his study, Katwebaze first checked to make sure that all the columns were numerical. He achieved this by using music_data["explicit"] = music_data["explicit"].astype(int) (Katwebaze, 2023). This was the only column in his dataset that required the conversion of words into numbers for analysis. One aspect of his analysis that stood out to me was the inclusion of the a trends graph. Katwebaze used the release dates to analyze trends in music by turning the data into time series graphs. This helped him understand if there were any trends in the data that a human eye would miss. Another part that stood out was how Katwebaze did not use PCA to reduce the dimensionality of the dataset. I did notice he imported the PCA model from sklearn; however, never employed its use into his study.

## Methodology
For my study, I first started out by gathering info on the dataset and exploring it. I quickly learned that the dataset used included four non-numerical columns. The next step I took was to use sklearns label encoder to convert each column into numbers. For example, the encoder converted pop to a one and country to two. [include picture]
The next step I took was to create a correlation matrix. I did this to help analyze if certain characteristics of songs correlated well. [include picture of matrix]
I then scaled down the data as I noticed there were almost 2500 different genres of music. I scaled the data down to make sure certain features did not outweigh the impact of others. This was done likewise in Katwebaze's study as well. 

## Results


## Discussion


## References
Katwebaze, E. (2023, February 9). Music recommendation system using KMeans & KNN. Kaggle. https://www.kaggle.com/code/emmanuelkatwebaze/music-recommendation-system-using-kmeans-knn 

(Katwebaze, 2023)
