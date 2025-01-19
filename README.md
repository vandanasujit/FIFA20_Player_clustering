# FIFA 20 Player Data Analysis and Clustering
## Overview
This project focuses on analyzing the FIFA 20 player dataset to gain insights into player skills, market value, and performance. Additionally, players are clustered based on their attributes, and several key questions related to player rankings, performance trends, and wages are answered. The dataset includes detailed information on players across multiple FIFA versions, from FIFA 15 to FIFA 20.

## Problem Statement
The project is divided into three tasks:

* ###### Task 1: Prepare a complete data analysis report on the given data.

* ###### Task 2: Explore football skills and cluster football players based on their attributes.

* ###### Task 3: Explore the data and answer the following questions:

1. Prepare a rank-ordered list of the top 10 countries with the most players. Which countries are producing the most footballers that play at this level?
2. Plot the distribution of overall rating vs. age of players. Interpret at what age players tend to stop improving.
3. Which type of offensive players tends to get paid the most: strikers, right-wingers, or left-wingers?
## Dataset
The dataset provided includes player data for the Career Mode from FIFA 15 to FIFA 20. It allows for multiple comparisons of the same players across these six versions of the game.

###### Dataset Source: Link : https://d3ilbtxij3aepc.cloudfront.net/projects/CDS-Capstone-Projects/PRCP-1004-Fifa20.zip

## Key Features:
Player Info: Name, Age, Nationality, Club, Position, Wage, Value, Overall Rating, Potential
Player Skills: Dribbling, Passing, Shooting, Defending, Physical, etc.
Player Performance over Time: Skill attributes across FIFA 15-20 for comparison

## Analysis and Exploration
* ###### Task 1: Data Analysis
The project begins with thorough data cleaning and preprocessing. Exploratory data analysis (EDA) is then performed to extract insights into player demographics, skill distribution, and salary trends.

* ###### Task 2: Clustering Players
Football players are clustered based on their attributes, allowing us to group players with similar skills and styles. The clustering helps understand different types of players and their unique characteristics.

* ###### Task 3: Answering Key Questions
Top 10 Countries with Most Players: A ranked list of countries producing the most players at this competitive level.
Overall Rating vs. Age: A distribution plot is created to analyze player performance over age and determine the point when players tend to stop improving.
Offensive Player Wages: A comparison of wages for different types of offensive players (striker, right-winger, left-winger) to see which position tends to be paid the most.
## Additional Ideas for Analysis
Some other potential analyses that could be done with the dataset include:

* Messi vs. Ronaldo: Historical comparison between Messi and Ronaldo, tracking changes in their attributes over time.
* Building a Competitive Team: Analyze the ideal budget required to build a competitive team and explore diminishing returns on player value.
* Trends in Player Attributes: Track how attributes like Agility, BallControl, and Strength have evolved among top players over different FIFA versions.
## Technologies Used
* Python: For data analysis and machine learning
* Pandas: For data manipulation and preprocessing
* Matplotlib and Seaborn: For data visualization
* Scikit-learn: For clustering analysis and modeling
* Jupyter Notebook: For interactive coding

## Results
* ##### Clustering:
   Players were successfully clustered into different groups based on their skill attributes. The models i used for clustering are:
1. ###### K-means
2. ###### DBscan
3. ###### Agglomerative Clustering.
 So among these Kmeans and agglomerative algorithm were better in creating the clusters and getting good score.
 For both these models I got approximatily 0.60 silhouette score. This score should be between 0.5 and 1 for a good model. 
* ##### Top 10 Countries:
  Identified the top countries producing the most players.
* ##### Player Age and Improvement:
   Found a specific age range where players tend to stop improving in terms of overall rating.
* ##### Offensive Players Wages:
  Discovered which offensive player positions tend to command the highest wages.

## Challenges Faced In This Project
* ###### Since this is a high dimensional dataset it was hard to analyse all the features of each player. I used correlation matrix and heatmap to overcome this.
* ###### Cleaning the dataset was challenging.It required understanding of business case and domain knowledge. To get it I had to refer to various resources on internet.
* ###### The cleaned dataset had 79 features after dropping the unwanted features, which is hard for K-means to find meaningfull cluster.As the number of dimensions increases, the distance between points tends to become similar, making it difficult to differentiate clusters. so to reduce the dimensionality I used PCA (Principal Component Analysis)  before applying KMeans.



