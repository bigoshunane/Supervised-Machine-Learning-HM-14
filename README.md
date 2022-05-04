# Supervised-Machine-Learning-Predicting Credit Risk.
The aim of this project is building a machine learning model that attempts to predict whether a loan from LendingClub will become high risk or not.

# Data Source
LendingClub (2019-2020) Loan Stats retrieved from: [https://resources.lendingclub.com]

# Background
LendingClub is a peer-to-peer lending services company that allows individual investors to partially fund personal loans as well as buy and sell notes backing the loans on a secondary market. LendingClub offers their previous data through an API.
You will be using this data to create machine learning models to classify the risk level of given loans. Specifically, you will be comparing the Logistic Regression model and Random Forest Classifier.

# Steps and Results
#  Loading data source
<img width="522" alt="g" src="https://user-images.githubusercontent.com/84547558/166557736-c985190d-0ecf-4b48-9128-789df00de8ae.png">

#  Convert categorical data to numeric and separate target feature for training and testing data
<img width="468" alt="2" src="https://user-images.githubusercontent.com/84547558/166558546-fa3fac9d-7c0e-4362-9534-ef6661684924.png">

#  Using LabelEncoder to convert output labels to binary (0 and 1)
<img width="619" alt="3" src="https://user-images.githubusercontent.com/84547558/166558764-184b817e-bbaa-46da-8769-85ebff81086e.png">

# Create Logistic Regression Model for the unscaled data

<img width="681" alt="5" src="https://user-images.githubusercontent.com/84547558/166559227-4996e653-dd3f-4e11-b5ea-4d1a3d5147fb.png">


# Create Confusion Matrix for the Logistic Regression Model for the unscaled data
<img width="628" alt="6" src="https://user-images.githubusercontent.com/84547558/166559438-58d09034-6c8d-4b70-864d-80b210d02610.png">

# Printing out the Classification Report
<img width="569" alt="7" src="https://user-images.githubusercontent.com/84547558/166559732-f46efe20-85d0-4e47-84a7-849b19497e6b.png">

# Visualizing the Confusion Matrix for the Logistic Regression Model
<img width="597" alt="8" src="https://user-images.githubusercontent.com/84547558/166560101-f1ad17bd-ecf4-408b-b0f7-141e40fad27f.png">
<img width="566" alt="9" src="https://user-images.githubusercontent.com/84547558/166560263-62399c06-5830-437b-92c7-3e834471d884.png">

# Repeat same steps as above for the scaled data
<img width="560" alt="a" src="https://user-images.githubusercontent.com/84547558/166560756-aa2ca466-1a55-4223-b162-519dd6c45a02.png">

# Training and Testing Score for scaled data (Logistic Regression Model)
<img width="499" alt="b" src="https://user-images.githubusercontent.com/84547558/166561065-751c358f-6a52-4a3f-9c13-552cd4a20da1.png">

# Classification Report for scaled data (Logistic Regression Model)
<img width="570" alt="c" src="https://user-images.githubusercontent.com/84547558/166561285-eedb9a3c-ebc9-439f-a451-6850fd4a839e.png">

# Confusion Matrix heatmap for scaled data (Logistic Regression Model)
<img width="467" alt="d" src="https://user-images.githubusercontent.com/84547558/166561440-7f37b6bc-0c25-40dd-ba08-7efd540319b3.png">

# Create Random Forest Classifier for the unscaled data
<img width="808" alt="f" src="https://user-images.githubusercontent.com/84547558/166561750-818dde8b-7db9-497d-b480-3733376e261f.png">

# Conclusion

# Random Forest Classifier
For unscaled data, the scores for the Random Forest Classifier Model:

      . Training Score: 1.0
      . Testing Score:  0.6180348787749894
      
For scaled data, the scores for the Random Forest Classifier Model:

     . Training Score: 1.0
     . Testing Score:  0.6193109315185028

From the scores above, the Random Forest Classifier won't be very efficient in predicting the Credit Risks. The differences between the scores on the scaled and unscaled data are almost identical (The difference is negligible).

# Logistic Regression Model
For the unscaled data, the scores for the Logistic Regression:

    . Training Data Score: 0.6485221674876848
    . Testing Data Score:  0.5253083794130158
For the scaled data, the scores for the Logistic Regression:

    . Training Data Score: 0.713136288998358
    . Testing Data Score:  0.7201190982560612
From the scores above, the best model to predict the Credit Risk is the Logistic Regression on the scaled data. The training scores and testing scores are much more closer than the unscaled data, hence giving more confidence to make a more accurate prediction.

Therefore, in conclusion, Logistic Regression will be a better model to use.

© 2021 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
