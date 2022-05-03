# Supervised-Machine-Learning-Predicting Credit Risk.
The aim of this project is building a machine learning model that attempts to predict whether a loan from LendingClub will become high risk or not.

# Data Source
LendingClub (2019-2020) Loan Stats. Retrieved from: [https://resources.lendingclub.com/]

# Background
LendingClub is a peer-to-peer lending services company that allows individual investors to partially fund personal loans as well as buy and sell notes backing the loans on a secondary market. LendingClub offers their previous data through an API.
You will be using this data to create machine learning models to classify the risk level of given loans. Specifically, you will be comparing the Logistic Regression model and Random Forest Classifier.

# Steps
# Loading data source
train_df = pd.read_csv(Path('Resources/2019loans.csv'))
test_df = pd.read_csv(Path('Resources/2020Q1loans.csv'))
