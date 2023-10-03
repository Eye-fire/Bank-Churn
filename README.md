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
db = pd.read_csv("C://Users/wawes/OneDrive/Desktop/ZETECH UNIVERSITY/Y4S2/MACHINE LEARNING/Topic 2/churn.csv")

Display a summary of the dataset to familiarize yourself with the data
db

View database structure to get the datatypes, number of entries and null values
db.info()

Convert data into a format that easily be used to perform comparisons and plotting 
def label_encoder(db_: pd.DataFrame(), columns_name_: list):
    le = LabelEncoder()
    for i in columns_name_:
        le.fit(db_[i])
        db_[i] = le.transform(db_[i])
    return db_

db = label_encoder(db, ['Geography', 'Gender'])
db

# Exploratory Data analysis
The following are the different techniques used to explore the data




