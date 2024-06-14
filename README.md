# Electricity Consumption Forecasting

This project aims to forecast the PJME (PJM Energy Market) hourly energy usage in megawatts (MW) using historical data and machine learning techniques. The process involves data preprocessing, feature engineering, outlier removal, time series cross-validation, and model training using the XGBoost algorithm. The final model predicts future energy consumption, and the results are visualized to evaluate the model's performance.

## Tools and Libraries

The following libraries and tools were used in this project:

- **Pandas:** For data manipulation and analysis.
- **Matplotlib:** For data visualization.
- **Seaborn:** For enhanced data visualization.
- **Numpy:** For numerical operations.
- **XGBoost:** For implementing the gradient boosting model.
- **Scikit-learn:** For model evaluation and time series cross-validation.

## Project Workflow

**1. Data Loading and Visualization**

- Load the dataset containing PJME hourly energy usage.
- Plot the time series data to visualize trends and patterns.

**2. Outlier Analysis and Removal**

- Identify and remove outliers in the dataset to improve model accuracy.
- Visualize the distribution of energy usage and filter out anomalies.

**3. Train-Test Split**

- Split the dataset into training and testing sets based on a specific date (01-01-2015).
- Visualize the train-test split to ensure correct partitioning.

**4. Time Series Cross-Validation**

- Implement time series cross-validation with 5 splits to evaluate model performance.
- Visualize each fold's train-test split to ensure proper cross-validation.

**5. Feature Engineering**

- Create new time-based features (hour, day of the week, month, year, etc.) to enhance model performance.
- Add lag features to incorporate historical energy usage information.

**6. Model Training and Evaluation**

- Train the XGBoost regressor using the created features and target variable.
- Evaluate model performance using root mean squared error (RMSE) across different folds.
- Visualize model predictions against actual values to assess accuracy.

**7. Future Predictions**

- Generate future time frames for prediction.
- Use the trained model to predict future energy usage.
- Visualize the future predictions to understand the model's forecast.

**8. Model Saving and Loading**

- Save the trained model to a file for future use.
- Load the saved model and test its prediction capability.

  
## Results

- The model achieved an average RMSE score of 3742.5833 across the validation folds.
- The trained model effectively captures the trend and seasonality in the PJME energy usage data.
- Future predictions indicate a reasonable forecast of energy usage, with visualizations supporting the model's accuracy.

## Conclusion

This project demonstrates the application of machine learning techniques to time series forecasting in the energy sector. The use of XGBoost and careful feature engineering resulted in a model capable of predicting future energy consumption with reasonable accuracy. Further improvements could be made by exploring additional features or different model architectures.

