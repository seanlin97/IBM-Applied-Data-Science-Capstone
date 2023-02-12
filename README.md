# Applied Data Science Capstone
The final assignment of Applied Data Science Capstone in IBM Data Science Professional Certificate.
The final report can be found above as a pdf file and part of it will be presented below.


## Review criteria
* Uploaded the URL of your GitHub repository including all the completed notebooks and Python files (1 pt)
* Uploaded your completed presentation in PDF format (1 pt)
* Completed the required Executive Summary slide (1 pt)
* Completed the required Introduction slide (1 pt)
* Completed the required data collection and data wrangling methodology related slides (1 pt)
* Completed the required EDA and interactive visual analytics methodology related slides (3 pts)
* Completed the required predictive analysis methodology related slides (1 pt)
* Completed the required EDA with visualization results slides (6 pts)
* Completed the required EDA with SQL results slides (10 pts)
* Completed the required interactive map with Folium results slides (3 pts)
* Completed the required Plotly Dash dashboard results slides (3 pts)
* Completed the required predictive analysis (classification) results slides (6 pts)
* Completed the required Conclusion slide (1 pts)
* Applied your creativity to improve the presentation beyond the template (1 pts)
* Displayed any innovative insights (1 pts)


## Outline
* Executive Summary
* Introduction
* Applied Methodologies
* Results
* Conclusion


## Executive Summary
* Predict successful or not the SpaceX Falcon 9 will be landed
* The research process includes:
  * Data collection and wrangling
  * Exploratory data analysis (EDA)
  * Interactive visual analytics
  * Predictive analysis using Machine Learning
* Conclusion:
  * Decision Tree model is the most affective in this research
  * Lower payload mass has better success rate
  * Launch sites tend to locate near Equator line and by the coast
  * Success rate has been improving 
  * KSC LC-39A has the highest success rate

## Introduction
* This capstone project aims to predict the success of SpaceX's Falcon 9 first stage landing. The company's low launch cost of 62 million dollars compared to other providers' cost of 165 million dollars or more is largely due to the reusable first stage. 
* The project will use public information and machine learning models to determine the success of the first stage landing and its cost, which can be used by other companies bidding against SpaceX for a rocket launch. 
* The main question being addressed is whether the set of features such as payload mass, launch site, orbit type, etc., will result in a successful landing of the Falcon 9 first stage.


## Applied Methodologies
### Data collection and data wrangling methodology
#### Data collection
* SpaceX API
  * Acquire data using SpaceX custom functions
* Web scraping from Wikipedia
  * Acquire date using BeautifulSoup from HTML response
#### Data wrangling
* Process, clean, and combine the data we previously retrieved 
* Create an extra column to label the landing results to "1" as succeed and "0" as failed
### EDA and interactive visual analytics methodology
#### Exploratory data analysis (EDA)
* Pandas & NumPy
  * Basic cleaning, calculating, and manipulating data
* SQL
  * Perform queries to display, list, or count data
#### Interactive visual analytics
* Matplotlib & Seaborn
  * Using scatter plots, bar charts, and line charts to present the relationships between attributes
* Folium
  * Plotting interactive maps, furthermore,  adding markers and line to display launch sites and their characteristics
* Dash
  * Create interactive site with dropdown list and slider to exhibit pie charts and scatter plots based on the input data from user
### Predictive analysis methodology using Scikit
* Standardize the data
* Split the data into training and testing sets
* Apply GridSearchCV on:
  * Logistic regression
  * Support vector machine (SVM)
  * Decision tree
  * K nearest neighbors (KNN)
* Calculate the accuracy on the test sets and exam the confusion matrix
* Conclude the best ML model using Jaccard_score and F1_score

