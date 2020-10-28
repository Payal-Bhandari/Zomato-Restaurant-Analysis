 
Problem Definition: Performing Explaratory Data Analysis and Regression Analysis to determining the rating of restaurants depending upon locality,
food ,reviews using Zomato Restaurant Dataset. 
1)Prerequisite: Install Anaconda Python, Jupyter Notebook, Ubuntu 18.04.
2)Software Requirement: Jupyter Notebook, Spyder on Ubuntu.
3)Hardware Requirement: 2GB RAM, 500 GB HDD
4)Objectives: To understand the parameters determining the rating of restaurants in bangalore by applying linear regression,decision tree regression
and random forest regression.
5)Outcomes: After completion of this assignment we can analyze the best
locality,menu list for building new restaurant in Bangalore.

Theory Concepts:
1. Explaratory Data Analysis
EDA stands for Exploratory Data Analysis. EDA is a critical first step in
analyzing the data from an experiment.
Here are the main reasons we use EDA:
• detection of mistakes
• checking of assumptions
• preliminary selection of appropriate models
• determining relationships among the explanatory variables, and
• assessing the direction and rough size of relationships between
explanatory and outcome variables.
⦁ Typical data format
⦁ The data from an experiment are generally collected into a
rectangular array (e.g., spreadsheet or database), most commonly
with one row per experimental subject and one column for each
subject identifier, outcome variable, and explanatory variable.

⦁ Each column contains the numeric values for a particular
quantitative variable or the levels for a categorical variable. (Some
more complicated experiments require a more complex data
layout.)
⦁ Exploratory data analysis techniques have been devised as an aid
in this situation. Most of these techniques work in part by hiding
certain aspects of the data while making other aspects clearer.

⦁ Types of EDA
⦁ Univariate non-graphical
⦁ Multivariate non-graphical
⦁ Univariate graphical
⦁ Multivariate graphical.

2. Data Cleaning
Step 1 : Import the Data-set
By using Pandas we import our data-set and the file I used here is .csv file It’s
not necessarily every-time you deal with CSV file, sometimes you deal with Html
or Xlsx(Excel file). However, to access and to use fastly we use CSV files
because of their light weights. After importing the dataset, you can see we use
head function This function returns the first n rows for the object based on
position. It is useful for quickly testing if your object has the right type of data in it.
By default it returns 5 rows.

Step 2 : Check out the Missing Values
The concept of missing values is important to understand in order to successfully
manage data. If the missing values are not handled properly by the researcher,
then he/she may end up drawing an inaccurate inference about the data. Due to
improper handling, the result obtained by the researcher will differ from ones
where the missing values are present.
Two ways to handle Missing Values:
1. This method commonly used to handle the null values.
Here, we either delete a particular row if it has a null value for a particular feature
and a particular column if it has more than 75% of missing values. This method 
is advised only when there are enough samples in the data set. One has to make
sure that after we have deleted the data, there is no addition of bias. Removing
the data will lead to loss of information which will not give the expected results
while predicting the output.

2. Drop the Missing Values
This strategy can be applied on a feature which has numeric data like the year
column or Home team goal column. We can calculate the mean, median or
mode of the feature and replace it with the missing values. This is an
approximation which can add variance to the data set. But the loss of the data
can be negated by this method which yields better results compared to removal
of rows and columns. Replacing with the above three approximations are a
statistical approach of handling the missing values. This method is also called as
leaking the data while training. Another way is to approximate it with the
deviation of neighbouring values. This works better if the data is linear.

Step 3: See the Categorical Values
Analyze the categorical values of column and assign the numeric values for each
category which can be useful in furthur processing of data and mapping of data.
Suppose we have gender as a column having values male and female then we
can assign 1 for male and 0 female using LabelEncoder class.

Step 4 : Splitting the data-set into Training and Test Set
In any Machine Learning model is that we’re going to split data-set into two
separate sets
1. Training Set
2. Test Set
Using train_test_split class we can split the given dataset into train and test data.
Train data is the input data for the processing and test data is the data used for
comparison with train data hence machine can predict on basis of this data.

3. Analysis

⦁ Linear Regression
linear regression is a linear approach to modeling the relationship
between a scalar response (or dependent variable) and one or more
explanatory variables (or independent variables).

⦁ Decision Tree Regression
Decision Tree - Regression. Decision tree builds regression or
classification models in the form of a tree structure. It breaks down a
dataset into smaller and smaller subsets while at the same time an
associated decision tree is incrementally developed.

⦁ Random Forest Generator
Random forests or random decision forests are an ensemble learning
method for classification, regression and other tasks that operates by
constructing a multitude of decision trees at training time and outputting
the class that is the mode of the classes (classification) or mean
prediction (regression).

# About the Data Set
The basic idea of analyzing the Zomato dataset is to get a fair idea about the
factors affecting the aggregate rating of each restaurant, establishment of
different types of restaurant at different places, Bengaluru being one such city
has more than 12,000 restaurants with restaurants serving dishes from all over
the world.
url contains the url of the restaurant in the zomato website
address contains the address of the restaurant in Bengaluru
name contains the name of the restaurant
online_order whether online ordering is available in the restaurant or not
book_table table book option available or not
rate contains the overall rating of the restaurant out of 5
votes contains total number of rating for the restaurant as of the above
mentioned date
phone contains the phone number of the restaurant
location contains the neighborhood in which the restaurant is located
rest_type restaurant type
dish_liked dishes people liked in the restaurant
cuisines food styles, separated by comma
approx_cost(for two people)contains the approximate cost for meal for two
people
reviews_list list of tuples containing reviews for the restaurant, each tuple
consists of two values, rating and review by the customer
menu_item contains list of menus available in the restaurant
listed_in(type) type of meal
listed_in(city) contains the neighborhood in which the restaurant is listed

We can ask the following questions
1. What kind of a food is more popular in a locality.
2. Do the entire locality loves vegetarian food. If yes then is that locality
populated by a particular sect of people for eg. Jain, Marwaris, Gujaratis who are
mostly vegetarian. These kind of analysis can be done using the data, by
studying the factors such as • Location of the restaurant • Approx Price of food
Theme based restaurant or not
3. Which locality of that city serves that cuisines with maximum number of
restaurants • The needs of people who are striving to get the best cuisine of the
neighborhood • Is a particular neighborhood famous for its own kind of food.

# Conclusion:
Thus, after successfully completing this assignment, we were able to understand
that the restuarants which are located in the central Bangalore have more visits
and the ratings of the restaurants is between 3 and 4.
