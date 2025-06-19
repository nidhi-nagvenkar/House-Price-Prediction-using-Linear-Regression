# House-Price-Prediction-using-Linear-Regression
This project applies Linear Regression, a supervised machine learning technique, to predict housing prices using a real-world dataset. The dataset contains various features of houses, and the goal is to train a model that can accurately estimate the selling price based on those features.

📊 Project Report
🔹 1. Data Preparation
Loaded the dataset (house_price_data.csv) using Pandas
Explored the dataset to understand the structure and data types
Checked for and handled missing values
Ensured that all input features were numerical
Defined the feature set X and the target variable y (Price)
Performed an 80/20 train-test split using train_test_split from sklearn

🔹 2. Model Building
Used LinearRegression from sklearn.linear_model
Trained the model on the training data using .fit()
Predicted prices for the test data using .predict()

🔹 3. Model Evaluation
Evaluated the model using:
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
R² Score (Coefficient of Determination)
Created scatter plots to visualize:
Actual vs. Predicted prices on training set
Actual vs. Predicted prices on test set

🔹 4. Results
The predicted prices were added directly into the test set using:
python
Copy
Edit
X_test['Actual Price'] = y_test.values
X_test['Predicted Price'] = y_pred
Visualization showed that most predicted values closely followed the actual prices, indicating that the model performed reasonably well.

📈 Technologies Used
Python
Jupyter Notebook
Pandas, NumPy, Matplotlib, Seaborn
Scikit-learn

🧠 Conclusion & Insights
The Linear Regression model provided a good baseline for predicting house prices.
While the model worked well, improvements could be made by:
Feature engineering
Removing outliers
Trying more advanced models like Decision Trees or Random Forests
