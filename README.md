# Exploratory Data analysis on database
# Introduction
Exploratory Data Analysis (EDA) is a process for investigating datasets, elucidating subjects, and visualizing the outcomes. EDA is an approach for data analysis that applies a diversity of techniques to maximize certain insights into a data set; reveal underlying structure; extract significant variables; detect outliers and anomalies; test underlying assumptions; develop models, and determine best parameters for future estimations. 
This assignment by Mr. Kega is built on providing practical knowledge about the main pillars of EDA including data cleaning, data preparation, data exploration, and data visualization.
The study will provide the opportunity to explore open-source datasets including bank churn and salaries datasets, and many others. Using these real-life datasets, to understand the data, summarize their characteristics, and visualize them for business intelligence. 
We will be using Pandas, a powerful library for working with data, and other core Python libraries including NumPy and SciPy, StatsModels for regression, and Matplotlib for visualization.

# Statement of the problem
We are using a database called Bank Churn to perform classification problems in order to highlight useful insights about the data and make informed decision

# Importance of solving the problem
Solving the problem enables us to create insights that lead to the development of learning models that can be used to learn and make predictions that are useful in the decision-making process.

# Data preparation
Load the dataset into the code
* db = pd.read_csv("C://Users/wawes/OneDrive/Desktop/ZETECH UNIVERSITY/Y4S2/MACHINE LEARNING/Topic 2/churn.csv")

Display a summary of the dataset to familiarize yourself with the data
* db

View the database structure to get the datatypes, number of entries, and null values
* db.info()

Convert data into a format that easily be used to perform comparisons and plotting 
* def label_encoder(db_: pd.DataFrame(), columns_name_: list):
    le = LabelEncoder()
    for i in columns_name_:
        le.fit(db_[i])
        db_[i] = le.transform(db_[i])
    return db_

* db = label_encoder(db, ['Geography', 'Gender'])
* db

# Exploratory Data analysis
The following are the different techniques used to explore the data

Plotting the credit score and balance to get an insight into the two variables
* mpl.scatter(db.CreditScore, db.Balance)
* mpl.title('Credit Score vs Balance')
* mpl.xlabel('CreditScore')
* mpl.ylabel('Balance')

Getting a summary of the population from different geographical regions
* db['Geography'].value_counts()

Classifying other variables from the dataset to get further insight into the dataset.

# Regression tests on Profesional Salaries Churn Dataset

# Statement of the problem
We are using the regression technique to predict future output for independent variables in the dataset

# Intorduction
Linear regression is a statistical method for modeling relationships between a dependent variable with a given set of independent variables.
Simple linear regression is an approach for predicting a response using a single feature. In linear regression, we assume that the two variables i.e. dependent and independent variables are linearly related. Hence, we try to find a linear function that predicts the response value(y) as accurately as possible as a function of the feature or independent variable(x). Let us consider a dataset where we have a value of response y for every feature x: 

the task is to find a line that fits best in the above scatter plot so that we can predict the response for any new feature values. (i.e a value of x not present in a dataset) This line is called a regression line.

# Data Preparations
We use the following steps in data preparations
* Load the data into the machine
* Display the summary to familiarize yourself with the dataset
* Converting some strings into floats to be used as independent and dependent variables
* Checking for null values and replacing them with zeros

# Exploratory Data Analysis
We plot some independent and dependent variables to get the prediction using the regression line


