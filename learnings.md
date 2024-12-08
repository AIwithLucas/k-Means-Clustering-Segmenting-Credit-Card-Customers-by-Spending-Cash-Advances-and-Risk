#### 1: Understanding purpose of Standard Scaler from scikit learn

    - to standardize features to have mean of 0 and standard deviation of 1
    - transforms data by subtracting the mean and dividing by standard deviation
    - ensures that all features contribute equally by removing scale-related bias in models
        - k-Means
        - Logistic Regression
        - SVM
    - models like kNN and Linear regression rely on distances between datapoints. larger magnitude features can dominate distance calculations
    - helps with faster convergence in gradient based models & better model accuracy

#### 2. Training kMeans clustering requires 2 dimensional array, so have to use X.reshape(-1, 1) to make it from 1D to 2D
