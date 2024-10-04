# Decision Tree Model for Heart Disease Prediction
This project demonstrates the steps involved in building a Decision Tree model to predict heart disease using a structured approach to data preprocessing, exploratory analysis, and model evaluation.

**Steps Involved**

1. Data Preparation and Exploratory Data Analysis (EDA)

Imported essential libraries: numpy, pandas, matplotlib, and seaborn.

Loaded the Dataset: The heart disease dataset was loaded and its attributes were understood.

Data Cleaning: Checked for null and duplicate values.

**EDA:**

Plotted distribution plots for numerical columns to understand data distribution.

Used countplots for categorical columns to gain insights on how variables influence the target.

Generated a heatmap to identify correlations (no strong correlation was found).

Used AutoViz and Sweetviz libraries for data quality checks and outlier detection.

2. Data Splitting

Split the dataset into training and test sets using train_test_split from Scikit-learn.

3. Model Building

Model Used: Imported DecisionTreeClassifier from sklearn.tree.

Training: Fit the model using the training data and made predictions.

Evaluation: Used accuracy_score, confusion_matrix, and classification_report to assess model performance.

The initial accuracy was 79%.

Confusion matrix and classification report provided insights into precision, recall, and F1 score for both target classes.

4. Hyperparameter Tuning

Applied GridSearchCV for hyperparameter tuning.

After tuning, the model accuracy improved slightly to 80%, but it wasn't significantly better than the original model.

5. Decision Tree Visualization

Installed and used the graphviz library to visualize the decision tree.

6. Conclusion

Achieving 79-80% accuracy is not ideal in the medical domain, especially for predicting severe diseases like heart disease, where an accuracy score of 95% or above is preferable.
Decision Tree may not be the best algorithm for this dataset. Other models, such as Random Forest, could potentially provide better accuracy.
