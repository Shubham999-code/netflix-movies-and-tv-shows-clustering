# Netflix-Movies-And-TV-Shows-Clustering :-
To ensure an optimal user experience and prevent subscriber churn, it is essential for Netflix, the world's leading online streaming service provider with over 220 million subscribers as of 2022, to effectively cluster the shows on their platform..
# Table of Content :-
1. Problem Statement
2. Objective
3. Dataset
4. Data Pipeline
5. Project Structure
6. Conclusion
# Problem Statement :-
This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.

In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.
# Objective :-
The objective of this project is to organize the Netflix shows into distinct clusters, where the shows within a cluster are alike and the shows in different clusters are dissimilar to one another.
# Dataset :- 
The dataset used in this project is sourced from Flixable, a third-party Netflix search engine. The data includes information on all movies and TV shows available on the streaming platform as of 2019, with a total of 7787 records and 12 attributes. Each attribute provides specific information about the movie or TV show.
# Data Pipeline :-
1. Know Your Data: The first step in this project was to examine the various features of the dataset, understand the structure of the data and identify any patterns or trends. We looked at the shape of the data, the data types of each feature, and a statistical summary.
2. Exploratory Data Analysis: We conducted an exploratory analysis of the data to identify patterns and dependencies, and to draw conclusions that would be useful for further processing.
3. Data Cleaning: We checked for duplicated values in the dataset and then addressed any null values and outliers by imputing empty strings and dropping some of the null rows.
4. Textual Data Preprocessing: We used techniques such as stop word removal, punctuation removal, conversion to lowercase, stemming, tokenization, and word vectorization to prepare the textual data for clustering. We also used Principal Component Analysis (PCA) to handle the curse of dimensionality.
5. Cluster Implementation: We used K-Means and Agglomerative Hierarchical clustering algorithms to cluster the movies and determine the optimal number of clusters.
6. Content-Based Recommendation System: We built a content-based recommendation system using the similarity matrix obtained from cosine similarity, which will provide the user with 10 recommendations based on the type of movie/show they have watched.
#Conclusion :-
1. This dataset has 7787 rows and 12 columns.

2. Dataset is free from duplicate values.

3. Director column has maximum percentage of null values almost 30%, followed by cast and country columns with 9.2 and 6.7 % of null values respectively.

4. All columns have data of object type except release_year which is integer type, which means we have only one numerical column in the dataset.

# Chart - 1.
In the chart we are found two category movies and TV shows.There are 69.1% (5377) are movies and 30.9% (2410) are TV shows out of the total 7787 contents. so hence the number of movies are maximum than TV shows on netlix dataset.

# Chart - 2.
The above graph shows top 10 actors who have worked in loads of movies and TV shows.

# Chart - 3.
1. Documentaries are the top most genre in the netflix movies.
2. Kids TV is the top most genre in netflix TV shows.

# Chart - 4.
This visual shows Jan suter and Raul Campos are the leading directors.

# Chart - 5.
Most of the movies were found to be released in the month of october, november, december and january.

# Chart - 6.
There is linear augmentation in the release of movies from the year 2015 with its peak in the year 2019 followed by a sudden downfall in the year 2021, which was due to covid (lockdown).

# Chart - 7.
Most of the movies have duration of 90 mins.
Most of the TV shows have one season, but this number goes on decreasing with increase in number seasons

# Chart - 8.
In the year 2019 more number of movies were released as compared to TV shows.

# Chart - 9.
United state have higher no. of content.

# Chart - 10.
Family, Life, Find, Love are the most used words in the description column.

# Chart - 11.
India has number of movies releases than TV shows followed by Egypt with highest movie releases and less TV shows.

# Chart - 12.
Netflix has more content in the adult section followed by teen section.
# Chart - 13( Correlation Heatmap).
United States and United Kingdom are closely alighned with their netflix target ages.

1. Maximum adult content is from Spain.
2. Maximum teen content is from India.
3. Maximum older kids content is from Japan.
4. Maximum kids content is from Canada.

# Chart - 14(Correlation Heatmap).
Movie release is not biased with respect to days or months, and no other relationship or trends can be observed from the pairplots.
# Conclusion of EDA :-
1.Netflix have ~70% of movies and 30% of TV_shows in 2019.

2.Comedy is most popular genre in Netflix, across all content.

3.Netflix focuses to add new content majorly towards end of current year and start of new year.

4.A sudden drop was obserbed after 2020 in count of new content, Which is because of covid pandemic.

5.India is on 2nd place as compared to content availability, maximum content is available for United states.

6.There are almost ~30% of netflix original movies and ~50 % TV-shows.

7. Content category and countries:

   a. Maximum adult content is from Spain.
   
   b. Maximum teen content is from India.
   
   c. Maximum older kids content is from Japan.
   
   d. Maximum kids content is from Canada.
   
All of this insights will be neccesary for business development and SWOT analysis.

Conclusion for clustering. We tried 5 models for ML i.e.

K-means clustering Elbow curve Hierarchical clustering Agglomerative clustering K-means clustering shows that '4' will be optimum no of clusters with the silhoutte score of 0.45. But we selected Optimum cluster number as 6 after Elbow curve cross validation.

Thus K-means clustering will be best for this data set.

Cosine based recommender system was working really well.
