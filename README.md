# Medical Insurance Cost Prediction

The provided Python code performs exploratory data analysis (EDA) and builds a linear regression model for a health insurance dataset. Here's a breakdown of the code:

1. **Importing Libraries:**
   - `numpy`, `pandas`, `matplotlib.pyplot`, `seaborn`: Libraries for numerical operations, data manipulation, and data visualization.
   - `train_test_split` from `sklearn.model_selection`: Used for splitting the dataset into training and testing sets.
   - `LinearRegression` from `sklearn.linear_model`: Used for building a linear regression model.
   - `metrics` from `sklearn`: Provides performance metrics for evaluating the model.

2. **Loading and Inspecting Data:**
   - Reads the insurance dataset from a CSV file named 'insurance.csv' into a Pandas DataFrame.
   - Displays the first few rows of the dataset and its information, including data types and null values.

3. **Data Preprocessing:**
   - Checks for null values in the dataset.
   - Converts categorical values in the 'region' column to numerical values.

4. **Correlation Analysis:**
   - Calculates the correlation matrix for the numerical features in the dataset.
   - Visualizes the correlation matrix using a heatmap.

5. **Data Visualization:**
   - Plots distribution plots and count plots for various features such as age, gender, BMI, number of children, smoker status, and region.

6. **Linear Regression Model:**
   - Divides the dataset into features (X) and the target variable (Y).
   - Initializes a linear regression model.
   - Splits the dataset into training and testing sets.
   - Trains the linear regression model on the training data.

7. **Model Evaluation:**
   - Makes predictions on the training set and calculates the R-squared score as the training error.
   - Makes predictions on the test set and calculates the R-squared score as the test error.

8. **Prediction on a Specific Data Point:**
   - Takes a specific input data point (features) and predicts the insurance charges using the trained model.
   - Compares the predicted value with the actual value from the test set for a specific index (126 in this case).

Note: The R-squared score is used as an evaluation metric, and the model is applied to predict insurance charges for a specific input data point from the test set.

Keep in mind that this code assumes a linear relationship between the features and the target variable, which might not be the case in all scenarios.
