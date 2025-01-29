# Walmart-Weekly-Sales-ML-Algorithm
The solution to One of Kaggle's Datasets: https://www.kaggle.com/datasets/yasserh/walmart-dataset <br />
An interactive Jupyter Cell for finding Weekly Sales based on input!<br />
Accuracy: 92.677%

## Key Components of Solution

1. ***Data Preprocessing:***
    1. Made numpy array of features from Holiday_flag to Unemployment. **Shape: (m, 5)**
    2. *Store is a categorical data* and cannot be quantized as an ordinal number and hence used one-hot encoding to form a 45 column ndarray for each shop, 1 representing presence and 0 for absence. **Shape: (m, 45)**
    3. Made another ndarray which extracted month, year as dates from data
    4. Concatenated important features, dates, one hot encoded shops and stored as X_train.
    5. Seperate ndarray for storing output of each examples and stored as y_train. Reshaped it into 2d array for matrix multiplications.
2. ***Training:***
    1. Standardized using z score: X_train and y_train for feature scaling
    2. **Mean Squared Error**
    3. **Gradient Descent**
    4. r2 score for accuracy metrics
    5. Interactive cell for predicting new weekly sales based on respective features.
3. Used numpy matrix multiplications for faster computations and cleaner code.