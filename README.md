# Exploratory Data analysis on database
# Introduction
Exploratory Data Analysis (EDA) is a process for investigating datasets, elucidating subjects, and visualizing the outcomes. EDA is an approach for data analysis that applies a diversity of techniques to maximize certain insights into a data set; reveal underlying structure; extract significant variables; detect outliers and anomalies; test underlying assumptions; develop models, and determine best parameters for future estimations. 
This assignment by Mr. Kega is built on providing practical knowledge about the main pillars of EDA including data cleaning, data preparation, data exploration, and data visualization.
The study will provide the opportunity to explore open-source datasets including bank churn and salaries datasets, and many others. Using these real-life datasets, to understand the data, summarize their characteristics, and visualize them for business intelligence. 
We will be using Pandas, a powerful library for working with data, and other core Python libraries including NumPy and SciPy, StatsModels for regression, and Matplotlib for visualization.

# Statement of the problem
We are using a database called Bank Churn to perform classification problems in order to highlight useful insights about the data and make informed decision

# Importance of solving the problem
Solving the problem enables us to create insights that lead to the development of learning models to determine the following parameters that cause customers to leave or stay

* RowNumber—corresponds to the record (row) number and has no effect on the output. contains random values and has no effect on customers leaving the bank.
* Surname—the surname of a customer has no impact on their decision to leave the bank.
* CreditScore—can have an effect on customer churn, since a customer with a higher credit score is less likely to leave the bank.
* Geography—a customer’s location can affect their decision to leave the bank.
* Gender—it’s interesting to explore whether gender plays a role in a customer leaving the bank
* Age—this is certainly relevant since older customers are less likely to leave their bank than younger ones.
* Tenure—refers to the number of years that the customer has been a client of the bank. Normally, older clients are more loyal and less likely to leave a bank
* Balance—also a very good indicator of customer churn, as people with a higher balance in their accounts are less likely to leave the bank compared to those with lower balances.
* NumOfProducts—refers to the number of products that a customer has purchased through the bank.
* HasCrCard—denotes whether or not a customer has a credit card. This column is also relevant since people with credit cards are less likely to leave the bank.
* IsActiveMember—active customers are less likely to leave the bank
* EstimatedSalary—as with balance, people with lower salaries are more likely to leave the bank compared to those with higher salaries.
* Exited—whether or not the customer left the bank.

# Data preparation
Load the dataset into the code
* db = pd.read_csv("C://Users/wawes/OneDrive/Desktop/ZETECH UNIVERSITY/Y4S2/MACHINE LEARNING/Topic 2/churn.csv")

Display a summary of the dataset to familiarize yourself with the data
* db

View the database structure to get the datatypes, number of entries, and null values
* db.info()

# Exploratory Data analysis
We create several graphical presentations that try to bring out the insights that might cause customers to leave or stay in the bank

# Regression tests on Profesional Salaries Churn Dataset

# Statement of the problem
We are using the regression technique to predict future output for independent variables in the dataset

# Introduction
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


