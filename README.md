In the LoanStatus project, the goal was to build a model that predicts loan status (approved or rejected) using machine learning algorithms

1. Data Loading
We loaded the data from a CSV file and used pandas, seaborn, and matplotlib libraries for data analysis and exploration.
2. Exploratory Data Analysis (EDA)
We displayed some samples from the dataset and examined unique columns and missing values.
We used visualizations like distributions and boxplots to understand the data better.
3. Data Cleaning
We removed the Loan_ID column as it was not needed for analysis.
We filled missing values for categorical data using the mode and for numerical data using the median.
4. Encoding Categorical Data
We used One-Hot Encoding to convert categorical columns into numerical columns.
We monitored the data containing zero values in the CoapplicantIncome column.
5. Data Scaling
We used StandardScaler to scale numerical values like ApplicantIncome and LoanAmount to ensure consistency during model training.
6. Models Used

Several machine learning models were applied to predict loan status:

Support Vector Classifier (SVC)

The model was trained and performance was measured using accuracy_score, with cross-validation used for performance verification.
Logistic Regression

A logistic regression model was built, and different parameters were experimented with using Grid Search to find the best settings.
The model was trained using the best parameters to achieve maximum accuracy.
Decision Tree Classifier

A model to classify loans using decision trees.
Random Forest Classifier

Used Random Forest with multiple parameter tuning via Grid Search to improve the model's performance.
Accuracy was measured, and the best parameters were identified.

7. Model Optimization Using Grid Search
GridSearchCV was used to enhance performance by tuning model parameters, such as the number of trees, their depth, and criteria for splitting nodes.


Results
The accuracy of each model was measured to determine the best model for predicting loan status.
After optimization, high accuracy was achieved using Random Forest.
