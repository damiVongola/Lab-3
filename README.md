# Lab-3
Install the following python packages needed for this Lab. I would advice that as practice for industry, you install these packages in a virtual environment.

`pip install -U scikit-learn` `pip install pandas` `pip install numpy` `pip install jupyterlab` `pip install matplotlib`

This is the third Lab for the class Introduction to Machine Learning DIT 45100 AIW01

You will be provided with some sample code in sample_code.ipynb that should be enough for you to complete the labs. The following tasks below are our objectives for the lab

You will be implementing the following algorithms we discussed in class:

- Knn Regression (17 marks)
  - Implement algorithm i.e: Using python libraries.
  - Use KNeighborsRegressor from sklearn
    - Without feature scaling
      - Get the mse and rsquared on the testing set (with k=10)
      - Find the k that gives the lowset mse for the problem. (Try k's from 1-40). Print best k found
      - Plot testing set mse as k increases. Plot from k=1 to k=40 (y-axis: testing set mse, x-axis: k)
      - Fit KnnRegressor with best k and get the mse and rsquared on testing set
    - With feature scaling (Use Standard Scaler)
      - Get the mse and rsquared on the testing set (with k=10)
      - Find the k that gives the lowest mse for the problem. (Try k's from 1-40). Print best k found
      - Plot testing set mse as k increases. Plot from k=1 to k=40 (y-axis: testing set mse, x-axis: k)
      - Fit KnnRegressor with best k and get the mse and rsquared on testing set
      
 - Decision Tree Regression (25 marks)
   - Implement algorithm i.e: Using python libraries.
   - Use DecisionTreeRegressor from sklearn
     - Get the mse and rsquared on the training set
     - Get the mse and rsquared on the testing set
     - Grid search decision tree hyperparameters for ***preprunning*** with mse as score
       - Print best_params and best_score
       - Use best estimator from grid search and calculate mse and rsquared on the training set
       - Use best estimator from grid search and calculate mse and rsquared on the testing set
       - Show dataframe for all Grid search results
     - Use cost_complexity_pruning_path function to get alpha's and impurities from the tree for ***postpruning***
       - Plot impurities against alpha's returned by the function (y-axis: impurities, x-axis: alpha)
       - Train Decision Trees with all alphas returned by the function and get the train mse and test mse
       - Plot train and test mse's against alphas (y-axis: mse, x-axis: alpha)
       - Grab and print the alpha that gives the smallest mse in the testing set
       - Use the best alpha and fit a decision tree
         - Get training mse and rsquared
         - Get testing mse and rsquared
         - Plot decision tree using alpha that gives the smallest mse
         
 - Knn Classification (17 marks)
   - Implement algorithm i.e: Using python libraries.
   - Use KNeighborsClassifier
     - Without feature scaling
       - Get the log loss and accuracy on the testing set (with k=5)
       - Find the k that gives the lowest log_loss for the problem. (Try k's from 1-40). Print best k found
       - Plot testing set log loss as k increases. Plot from k=1 to k=40 (y-axis: testing set log loss, x-axis: k)
       - Fit KNeighborsClassifier with best k and get the log_loss and accuracy on testing set
     - With feature scaling (Use Standard Scaler)
       - Get the log loss and accuracy on the testing set (with k=5)
       - Find the k that gives the lowest log_loss for the problem. (Try k's from 1-40). Print best k found
       - Plot testing set log loss as k increases. Plot from k=1 to k=40 (y-axis: testing set log loss, x-axis: k)
       - Fit KNeighborsClassifier with best k and get the log_loss and accuracy on testing set
       
- Decision Tree Classification (25 marks)
  - Implement algorithm i.e: Using python libraries.
  - Use DecisionTreeClassifier from sklearn
  - Get the log loss and accuracy on the training set
  - Get the log loss and accuracy on the testing set
  - Grid search decision tree hyperparameters for ***preprunning*** with log_loss as score
    - Print best_params and best_score
    - Use best estimator from grid search and calculate log_loss and accuracy on the training set
    - Use best estimator from grid search and calculate log_loss and accuracy on the testing set
    - Show dataframe for all Grid search results
  - Use cost_complexity_pruning_path function to get alpha's and impurities from the tree for ***postpruning***
   - Plot impurities against alpha's returned by the function (y-axis: impurities, x-axis: alpha)
   - Train Decision Trees with all alphas returned by the function and get the train mse and test mse
   - Plot train and test log_loss against alphas (y-axis: log_loss, x-axis: alpha)
   - Grab and print the alpha that gives the smallest log_loss in the testing set
   - Use the best alpha and fit a decision tree
     - Get training log_loss and accuracy
     - Get testing log_loss and accuracy
     - Plot decision tree using alpha that gives the smallest log_loss
     
 - Linear Discriminant Analysis (3 marks)
   - Implement algorithm i.e: Using python libraries.
   - Calculate log_loss and accuracy on testing set
   
 - Quadratic Discriminant Analysis (3 marks)
   - Implement algorithm i.e: Using python libraries.
   - Calculate log_loss and accuracy on testing set
   
 - Gaussian Naive Bayes (5 marks)
   - Implement algorithm i.e: Using python libraries.
   - Without Feature Scaling
     - Calculate log_loss and accuracy on testing set
   - With Feature Scaling (Use Standard Scaler)
     - Calculate log_loss and accuracy on testing set
 
 - Multinomial Naive Bayes (5 marks)
   - Implement algorithm i.e: Using python libraries.
   - Without Feature Scaling
     - Calculate log_loss and accuracy on testing set
   - With Feature Scaling (Use MinMaxScaler)
     - Calculate log_loss and accuracy on testing set
         
        
