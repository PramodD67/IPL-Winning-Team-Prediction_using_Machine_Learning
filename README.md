# IPL-Winning-Team-Prediction_using_Machine_Learning

The aim of this project is to predict the  winning teams of IPL match 2021 on a  given a set of features as inputs. Input variables are team 1 , team 2 ,city And the output variable is winner. We are dealing only with winner. We have winner   between two team. The higher the value the better is winner. In this project we will treat each team  separately and their aim is to be able and find the winner of the match that work well for new unseen data. These are the classifiers.
Our IPL dataset contains match by match records from the first match played in the 2008 season till the complete 2020 season.
 In this project we are explaining the steps we followed to predict winner of IPL 2021, the study of data to extract knowledge and insights from the data and apply knowledge and actionable insights. In this project, we will work on IPL Data Analysis and Visualization Project using Python where we will explore interesting insights from the data of IPL matches like most run by a player, most wicket taken by a player, and much more from IPL season 2008-2020. We will initially perform simple statistical analysis and then slowly build to more advanced analysis

# DATA ACQUISITION AND CLEANING  

We are using Two datasets in this project, One dataset containing 2008 -2020 IPL Matches used for training the model and another dataset containing 2021 IPL Matches. The inputs are team names information, such as team1, team2 , city and the output is based on the team which has high winning probability.
The dataset provides the team names and , Season ,City ,Date ,Team1 ,Team2 ,Toss_winner ,Toss_decision ,Result, dl applied  Win_by_wicket, Win_by_runs,
Player_of_match, Umpire1, Umpire2 etc. 

Input variables based on given data set: 
•	Team1
•	Team2
•	City

Output variable based on sensory data: 
•	Winner


# DATA CLEANING
Data cleaning is the process of fixing or removing incorrect, corrupted, incorrectly formatted, duplicate, or incomplete data within a dataset. When combining multiple data sources, there are many opportunities for data to be duplicated or mislabeled. If data is incorrect, outcomes and algorithms are unreliable, even though they may look correct. There is no one absolute way to prescribe the exact steps in the data cleaning process because the processes will vary from dataset to dataset. But it is crucial to establish a template for data cleaning process. We applied Data cleaning on some unwanted columns. But before data cleaning some explorations and data visualization were applied on the data set using this it gave us an idea on how to deal with missing values and also extreme values.
We analysed the dataset and decided to remove some of the unwanted columns which are not useful for our prediction.  Such columns are :  

•	date
•	toss_winner
•	toss_decision
•	result
•	dl_applied
•	win_by_wickets
•	win_by_runs
•	player_of match
•	umpire1
•	umpire2
•	umpire3

# DATA VISUALIZATION 
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data. In the world of Big Data, data visualization tools and technologies are essential to analyze massive amounts of information and make data-driven decisions.
Data Visualization provides a clear understanding of the data. The information acquired in this section may be used during the modelling phase. 
Although UCI provides the dataset ready for analysis, it’s good practice to check it for possible issues we may encounter in the future. 
 Now, with a basic understanding of the attributes let us now start our project of data analysis and visualization of the IPL dataset with Python. We will initially perform simple statistical analysis and then slowly build to more advanced analysis.. 



# DATA MODELLING 
The process of modelling means training a machine learning algorithm to predict the labels from the features, tuning it for the business need, and validating it on holdout data.
Linear  Model : We Firstly use Linear Regression to predict the winning team for provided two different teams. This model establish relationship between independent and dependent variables by fitting a best line. This best fit line is known as regression line and represented by a linear equation Y= a *X +b. After applying the Linear Model the Prediction Accuracy we got was 29.628%. It seems the model is less accurate for prediction.

# Logistic Model:  Logistic Regression is used to estimate discrete values ( Binary values like 0/1, yes/no, true/false ) based on given set of independent variables. In simple words, it predicts the probability of occurrence of an event by fitting data to a logistic function. Since, it predicts the probability, its output values lies between 0 and 1. We use this model to predict the winning team for the provided two different teams. After applying the Logistic Model the Prediction Accuracy we got was 23.48%. It seems the model is less accurate than Logistic regression for prediction.

# KNN Model:  It can be used for both classification and regression problems. However, it is more widely used in classification problems in the industry. K nearest neighbors is a simple algorithm that stores all available cases and classifies new cases by a majority vote of its k neighbors. The case being assigned to the class is most common amongst its K nearest neighbors measured by a distance function. We use this model to predict the winning team for the provided two different teams. After applying the KNN Model the Prediction Accuracy we got was 61.56%. It seems the model is more accurate for prediction than Linear and Logistic regression models.

# Random Forest:
Random forests improve prediction performance over classification trees by averaging multiple decision trees. The algorithm creates several random subsets of the original data, in this case the training set, and calculates the classification trees, then the final result is the average of all trees. The name random forest derives from the random process of splitting the data and creating many trees, or a forest. After applying the Random Forest Model the Prediction Accuracy we got was 80.66%. It seems the model is more accurate for prediction than Linear, Logistic regression and KNN models that we applied previously.


# TESTING 
We are using two datasets in this project, One dataset containing 2008 -2020 IPL Matches used for training the model and another dataset containing only 2021 IPL Matches schedule. 2008-2020 IPL match dataset consists more than 800 matches which is used for training.
2021  2nd phase IPL match dataset nearly 27 matches which is used for testing using different classification and regression algorithms.






