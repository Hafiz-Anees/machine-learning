## for making machine learning project complete

1. dataset

2. divide the features into independent(2D array) and dependent (1D array)

3. train_test_split of dataset

4. standardization of dataset > fit_transform on training set and transform on test set

    - how to calculate x-score for standardization for training set
        z-score = (x - mean of training) / std
    - how to calculate x-score for standardization for test set
        z-score = (x - mean of training set) / std of training set

5. visualize the training set X_train and y_train

6. create the model and train the model

7. visualize the training set X_train and y_train with prediction line

8. predict the values for X_test

9. visualize the test set X_test and y_test with prediction line

10. compute the performance metrics mse , mae , rmse ,r2_score

     ## how to compute mse , mae , rmse , and r2_score mathmatically
        - mse = sum((y_test - y_pred)^2)
        - mae = sum(|y_test - y_pred|)
        - rmse = sqrt(mse)
        - r2_score = 1 - (sum((y_test - y_pred)^2) / sum((y_test - mean of y_test)^2))
        - adjusted r2 score = 1 - (1-r2_score)*(n-1)/(n-p-1)
            - n = number of observations(rows) in test set
            - p = number of features(columns) in test set

            
11. Assumptions checking for linear regression
    - linear relationship between y_test and y_pred
    - residuals should be normally distributed
    - homoscedasticity (constant variance) of residuals
    - no autocorrelation of residuals
    - no multicollinearity (for multiple linear regression)

12. how to deploy this model
    1. `Pickling` → Saving a Python object into a file (binary format).
    2. `Unpickling` → Loading the saved object back into memory