# Anime Recommender System: Project Overview
- Created a tool that recommends anime similar to the interest of the users who watches anime over various OTT platform 
- Scraped over 1 lakh anime descriptions
- Feature engineered the User's profile i.e their favourite aspects of the anime

# Code and Resources Used
- Python Version: 3.7
- Packages: pandas, numpy, matplotlib, seaborn
- Scraper Dataset: https://github.com/BhartiPandit98/Anime_recommender_system/blob/main/anime.csv

# Dataset Description
With each anime, we got the following:
- Anime Id - Unique identifier of each anime
- Name - Name of the anime
- Genre - Comma separated list of genres for this anime
- Type -  Movie, TV, OVA, etc
- Episodes - How many episodes in this show (1 if movie)
- Rating - Average rating out of 10 for this anime
- Members - Number of community members that are in this anime's "group"

# Data Cleaning
- Made columns for if different genres were present in the anime
- Imputed the missing values in genre with their mode value
- Found the genres of the user input anime and merged them together

# EDA



# Model Building
First, I seperated the genres corresponding to movie id. After merging user input with the genre, the rating of the user and the genre of each anime was multiplied and average was taken in order to get the user's weighted rating of the genres.
In order to give recommendation the weighted rating of the genre was multiplied by the genre of each anime and then sorted in descending order to give the top 5 recommendations.
