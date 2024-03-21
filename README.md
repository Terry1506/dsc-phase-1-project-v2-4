# Phase 1 Project Description
## 1.Introduction
 
 ## Overview of the project
 Microsoft wants to venture into the business of creating movies and do well in it.
 For this project we will use exploratory data analysis to generate insights for Microsoft's New Movie  Studios.
 ## Business Understanding
Microsoft has recognized the potential in the booming industry of original video content creation and has decided to venture into the  film production by establishing a new movie studio that will be calledMicrosoft's Movie Studios. However, due to lack of prior experience in this field, Microsoft seeks to gain a deeper understanding of the current trends and preferences that bring about success in the movie industry.

This project aims to conduct comprehensive research and analysis of the film market, focusing on identifying the genres that are performing exceptionally well at the box office. By examining box office data, audience demographics, critical reception by the audience, and how the worldwide gross and runtime of the movies, the project seeks to uncover insights into the attributes of successful movies.
## Objectives
i.  Loading datasets into pandas

ii.  Retrieving data from a DataFrame

iii.  Data preparation annd cleaning

iv.  Exploratory analysis

v.  Data visualization

## The analysis below should be able to answer the following questions:

1. What are the popular genres in the box office?
 2. Does popularity affect the worldwide gross?
3. Does rating affect the revenue?
4. Does popularity affect the ratings?

 ## Importing the relevant libraries
Begin by importing pandas, numpy, zipfile, csv with their aliases

#Your code here - remember to use markdown cells for comments as well! #importing libraries import pandas as pd br import sqlite3 import csv import numpy as np from datetime import datetime, import zipfile #importing data visualisation tools import matplotlib.pyplot as plt import seaborn as sns
%matplotlib inline
## Loading the datasets
To load the data we'll use:

movie_budget = pd.read_csv('zippedData/tn.movie_budgets.csv')
movie_gross = pd.read_csv('zippedData/bom.movie_gross.csv')
tmdb_movie = pd.read_csv('zippedData/tmdb.movies.csv',index_col=0)
reviews = pd.read_csv('zippedData/rt.reviews.tsv', delimiter='\t',encoding='unicode_escape')
conn = sqlite3.connect('zippedData/im.db')
movie_info = pd.read_csv('zippedData/rt.movie_info.tsv', delimiter ='\t', encoding='unicode_escape' )
## Data Visualizations!
[alt text](image-1.png)
![alt text](image-2.png)
![alt text](image-3.png)
![alt text](image-4.png)

 ## Conclusion
High rated movies gross higher, hence high profit margins.
Popular movies have a higher worldwide gross.
Popular movies have high ratings.
Drama, Comedy and Action genre of movies are the best to venture into since they are the popular genres.
## Recommendations
 1. Microsoft should come up with movies that incorporate drama, Action and comedy.
 2. Microsoft should come up with a strong marketing strategy  by allocating resources towards producing a diverse range of movies within the popular genres. Conduct market research to identify specific sub-genres or niche audiences within each genre to target, thereby maximizing the potential for worldwide gross and profit margins. since popularity increases the ratings and profits.
 3. Microsoft should focus on Quality Content: Invest in producing high-quality movies with strong storytelling, compelling characters, and engaging narratives. While high ratings are correlated with higher financial success, prioritizing quality content can help ensure positive critical reception and audience satisfaction, leading to higher profitability in the long run.







