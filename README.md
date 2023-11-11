# Netflix-Movies-and-Tv-shows-Clustering
![--------------------------------------------------------------------------------------------](https://github.com/andreasbm/readme/blob/master/assets/lines/grass.png)

### This repository includes the dataset and a research notebook presenting various approaches for clustering movies and TV shows within the Netflix dataset. The dataset encompasses movies and TV shows released between 1925 and 2021.
![--------------------------------------------------------------------------------------------](https://github.com/andreasbm/readme/blob/master/assets/lines/grass.png)


![N|Solid](https://media.tenor.com/twG41IiAAscAAAAC/no.gif)
# Problem Statement
The dataset we currently possess contains information about TV shows and movies accessible on Netflix as of 2019. This data was obtained from Flixable, an external Netflix search engine.

A compelling report from 2018 provided intriguing statistics about Netflix's content landscape. According to this report, the number of TV shows on Netflix had nearly tripled since 2010, while the count of movies had decreased by over 2,000 titles within the same timeframe. This shift underscores a significant transformation in the platform's content focus, with a notable emphasis on TV shows.

Further exploration of this dataset presents an exciting opportunity to uncover additional insights. By incorporating external datasets, such as IMDB ratings and Rotten Tomatoes scores, we can delve deeper into the quality and reception of the content offered by Netflix. This integration opens up avenues for discovering compelling findings and gaining a more comprehensive understanding of the platform's content offerings.
# Project Summary 
Netflix is an online platform that offers subscription-based streaming services for entertainment, encompassing a diverse selection of content, mainly categorized into movies and television shows. Over the years, it has emerged as the most popular Over-The-Top (OTT) platform globally, accessible to individuals worldwide. Despite the option for customers to terminate their memberships at any time, maintaining user interest is crucial for the company. This underscores the importance of recommendation systems, which play a key role in providing relevant suggestions to users.

As a media distribution corporation, Netflix originated with DVD delivery by mail and has since evolved significantly, focusing primarily on video streaming. The content available on the platform includes licensed material as well as original productions.

While Netflix initially emphasized movies, television series have become a more prominent genre in recent times. Operating on a subscription model, Netflix grants customers unlimited access to its content for a fee.

This project involves working with Netflix data to discern recent trends and gain insights into the presented material, sourced from Flixable, a third-party Netflix search engine. Notably, an analysis by Flixable in 2018 revealed a significant increase in the number of TV series on Netflix since 2010, while the number of movies decreased. This prompted the need for a recommendation system, which we developed by evaluating the data and clustering similar content based on text-based attributes.

Key steps in the project include:

1. Exploring the dataset by examining its head and tail.

2. Describing the dataset by calculating mean, minimum, maximum, and data types of columns.

3. Extracting information about non-null counts in column values.

4. Counting distinct values in each column.

5. Determining the shape of the dataset (number of rows and columns).

6. Addressing null values in certain columns by filling them with mode or replacing them with 'No Cast.'

7. Plotting relevant graphs to extract information.

8. Implementing Natural Language Processing (NLP) techniques, such as tokenization, punctuation removal, stopword removal, and word stemming.

9. Employing clustering models like K-means Clustering and Agglomerative Clustering.

10. Utilizing techniques like the Elbow method, Silhouette Score, and Dendrogram to determine the number of clusters in K-means.

11. Developing a recommendation system using K-means clustering results.

The project successfully conducted Exploratory Data Analysis (EDA), revealing critical findings to address significant business challenges. The implemented models, particularly K-means clustering, performed well despite the data's volume and complexity.
### Data Source:
- [Dataset](https://drive.google.com/file/d/17ecyUUnRHmssQzebQjnW7IUjKrRTC4oI/view?usp=sharing) - Dataset taken from AlmaBetter
# Conclusions for Machine learning models
The Elbow graph enabled us to identify the number of clusters, ultimately determining it to be 18. This number was discerned by locating a pronounced bend in the curve or a significant deviation from a straight line on the graph. The point on the x-axis corresponding to this juncture was selected as the value indicating the number of clusters.

Additionally, we employed the Silhouette score method, and upon evaluating the Silhouette Score, we found that the optimal score, amounting to 0.010383798598527266, was achieved with 15 clusters.

To ascertain the ideal number of clusters for K-means from another perspective, we examined the dendrogram. This involved identifying the longest vertical distance that could be drawn without intersecting any other horizontal lines and noting the number of vertical lines crossed after traversing this distance. According to the dendrogram's perspective, 15 clusters emerged as the optimum number for K-means.

The clustering of text-based features allows Netflix users to organize similar content preferences. By recognizing patterns and offering personalized recommendations, well-defined clusters enhance the recommendation system, thereby improving the overall user experience and content relevance on the platform.

