# sales-predictions-model
The code forecasts customer sales using time series analysis and a Random Forest model. It preprocesses sales data, creates lagged features, trains the model, predicts future sales, evaluates performance, and visualizes the results. The final output is a CSV file with sales predictions for each customer.


Purpose: The code aims to forecast customer sales for the next 12 months using a time series analysis approach. It primarily uses a Random Forest Regression model to predict future sales based on historical data.

Steps:
Data Loading and Preprocessing: The code starts by loading sales data from a CSV file, converts the 'date' column to a datetime format, and calculates monthly sales. It then creates a 'sales_diff' column to make the data stationary, which is essential for time series forecasting.
Supervised Data Preparation: The code prepares the data for supervised learning by creating lagged features (month_1, month_2, etc.) representing sales differences from previous months.

Train-Test Split: The data is split into training and testing sets to evaluate the model's performance.
Model Training: A Random Forest Regression model is trained on the training data.
Prediction: The model is used to predict sales for the next 12 months. These predictions are then combined with actual sales to provide the final forecasted sales.
Evaluation: The code evaluates the model using metrics like Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and R-squared (R2).
Visualization: A plot is generated to visualize the predicted sales against the actual sales.
Output: Finally, the code creates a new DataFrame with the predicted sales for each customer and saves it to a CSV file.

Key Libraries and Techniques:
Pandas and NumPy for data manipulation
Matplotlib for visualization
Scikit-learn for data preprocessing and model evaluation
Random Forest Regressor from scikit-learn for time series forecasting

Overall: The code provides a comprehensive workflow for time series forecasting, demonstrating data preprocessing, model training, evaluation, and visualization steps. It employs the Random Forest Regression model, known for its ability to handle complex relationships in data. The generated forecast helps in understanding future sales trends and planning business strategies.
I hope this description is helpful! Let me know if you have any other questions.
