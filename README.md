# Netflix-movies-and-tv-show-data-clustering
Analyzing the Netflix data to do clustering

AlmaBetter Capstone Project - Unsupervised: Netflix Movies And Tv Shows Clustering.

![image](https://github.com/lalitharode/netflix-movies-and-tv-show-data-clustering/assets/118443225/fa8505e8-fa93-4659-adf1-7768dc3b6946)
![image](https://github.com/lalitharode/netflix-movies-and-tv-show-data-clustering/assets/118443225/ce63dc63-5ffb-4e2b-b023-ecafd1574cf9)


# 📋 Introduction -

Netflix Inc. is an American media company based in Los Gatos, California. Founded in 1997 by Reed Hastings and Marc Randolph in Scotts Valley, California, it operates the over-the-top subscription video-on-demand service Netflix brand, which includes original films and television series commissioned or acquired by the company, and third-party content licensed from other distributors. (Wikipedia).

# 📋 Project summary -
This dataset consists of tv shows and movies available on Netflix. The dataset is collected from Flexible which is a third-party Netflix search engine. Netflix movies and TV shows clustering is a data analysis and machine learning technique that Netflix uses to group its content into similar categories. This technique involves analyzing the various characteristics of each title, such as genre, cast, and plot, and using algorithms to identify patterns and similarities. In essence, it's a set of algorithms using machine learning to analyze user data and movie ratings. To make it more effective, Netflix has set up 1,300 recommendation clusters based on users viewing preferences. Netflix's target market is young, tech-savvy users and anyone with digital connectivity. The audience of Netflix is from diverse age groups and demographics. However, most of the audience are teenagers, college-goers, entrepreneurs, working professionals, etc. Netflix's target consumers are divided into segments based on demographics, behavioral intents, and psychographic segmentation. Like most licensing agreements, the deal is structured in a traditional form, whereby Netflix pays for each film determined by rate cards on a sliding scale by each title's domestic or worldwide box office receipts. Netflix uses machine learning and algorithms to help break viewers' preconceived notions and find shows that they might not have initially chosen. To do this, it looks at nuanced threads within the content, rather than relying on broad genres to make its predictions.

# 📋 Dataset summary -

This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine. In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset. Integrating this dataset with other external datasets such as IMDB ratings, and rotten tomatoes can also provide many interesting findings.



We have the data which contains details of customers like id, age, and gender and also contains the details of the customer's vehicle

Dataset info:

Number of records: 7787

Number of features: 12

Features information:

The dataset contains features like:

show_id : Unique ID for every Movie / Tv Show

type : A Movie or TV Show

title : Title of the Movie / Tv Shows

director : Director of the Movie

cast : Actors involved in the movie / show

country : Country where the movie / show was produced

date_added : Date it was added on Netflix

release_year : Actual Release year of the movie / show

rating : TV Rating of the movie / show

duration : Total Duration - in minutes or number of seasons

listed_in : Generes

description: The Summary description

Project Workflow:

Importing Libraries,
Loading the dataset,
Data Summary,
Data Cleaning & Data Analysis,
Feature selection,
Implementing different clustering methods,
Conclusion,

# 📋 Visualization -

from the dataset, 30% of the content are from tv shows and 70% from movies. rating adult is usually present in maximum content either movies/tv shows.Since the number of movie shows is higher than the number of TV shows, movie shows receive the highest rating when compared to TV shows, from this we can say people like to watch movie show than compare to tv shows.

Over the years, Netflix has added more shows to its platform. Most movies were released in 2017 and 2018. Most television shows were broadcast in 2019 and 2020. The covid-19-induced lockdowns that stopped the production of shows may be to blame for the decline in the number of movies added in the year 2020. There are fewer movies uploaded this year because the Netflix data we have only extends through 2021.

Movies added counts are showing more as compared to tv shows. It looks that Netflix has prioritised adding more movie material over TV shows. The growth of movies has been significantly more pronounced than that of TV shows.

The majority of movies durations last between 90 and 120 minutes. Most tv shows have just one season. The pie plot visualisations show that the United States and India are the two countries that produce the most content.

# 📋 Preprocessing -

The cast, country, genre, and description are chosen as the attributes to cluster the data based on. These attributes' values underwent tokenization, preprocessing, and vectorization using TFIDF vectorizer.A total of 10000 characteristics were produced through TFIDF vectorization. For the purpose of overcoming the dimensionality curse, we applied Principal Component Analysis (PCA). 3000 components were able to capture more than 80% of variance.

# 📋 model used -

  1. Silhouette score, elbow method
  2. Agglomerative clustering
  3.  Recommended system

with the help of silhouette score and elbow method I found an idle number of clusters are 5. The Agglomerative clustering technique was then used to create clusters, with 5 being the optimum number. The dendrogram was visualized to achieve this. The similarity matrix acquired after utilizing cosine similarity was used to construct a content-based recommender system. Based on the sort of show the user viewed, this recommender system will provide them with 10 recommendations.
