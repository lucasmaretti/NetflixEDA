# NetflixEDA
Repository for files related to the exploratory data analysis of Netflix open data. This project is related to Udacity's Data Science Nanodegree project on Writing a data science blog post.

Github link to repository: https://github.com/lucasmaretti/NetflixEDA

# Installation

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python. The code should run with no issues using Python versions 3.*.

# Project motivation

## 1. Business Understanding
Netflix is one of the most popular movie / TV show streaming platforms in the market. Founded in 1997 as a mail DVD delivery service, it has grown to become a titan in the streaming business. This dataset was collected and made available on Kaggle by Flixable  which is a third-party Netflix search engine and contains detailed information on the content (movies and tv shows) added on the platform since 2008. This includes informations such as genres of the production, in which country it was produce, ratings and others.  By doing an initial exploration of the dataset the main question that drove the analysis was:
1. What can we learn by analyzing Netflix’s open data about its huge success over the recent years?
The next 2 questions came as a consequence of that:
2. Which are the countries that contribute the most to content production?
3. Which sector of audience do these countries target the most?

## 2.Data Understanding
The dataset has 7787 rows and 12 columns, each row representing a specific content (movie or tv show) on Netflix. There were few null columns, mainly on director and cast variables. Since these were not necessary for the analysis proposed, they were dropped.
## 3.Prepare Data
It was necessary some work to fix data types, such as date/time. Some columns, such as genre, are multilabel. To work with those, the Multilabel Binarizer package from scikit learn was used to transform the dataframe for that particular analysis. Also, since most of the variables are string / categorical, some Regex work was needed to fix some columns so that they were in a format adequate to work with the visualizations.
## 4.Data Modeling
Each question was answered via exploratory data analysis and visualizations - no model was deployed

## 5. Evaluation/ Results
The main findings of the code can be found at the post available here: https://lucasmaretti.medium.com/understanding-netflixs-growth-over-the-years-4217efbd827b.

# File descriptions
There is one notebook available here to showcase the work related the exploratory data analysis. Markdown cells were used to assist in walking through the thought process for individual steps.

# Licensing, authors and acknowledgments
You can find the Licensing for the data and other descriptive information at the Kaggle link available here: https://www.kaggle.com/shivamb/netflix-shows. 
