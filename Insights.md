# Findings and Insights  

Through comprehensive analyses, the initial goal was to forecast ATM cash demand to optimize cash management and minimize operational costs. The findings provided valuable insights into the effectiveness of different forecasting models, including SARIMA, Prophet, and Artificial Neural Networks (ANN). These insights demonstrated the potential of data analytics to drive smarter decision-making in financial operations, ensuring accurate predictions and efficient cash management.       

## Model Selection and Application
### SARIMA Model  

The SARIMA model was chosen for its robustness in handling datasets with seasonal and non-seasonal components. The model required the data to be stationary, which was achieved through log transformation and first-order differencing. Stationarity tests such as the Augmented Dickey-Fuller (ADF) test and KPSS test confirmed the data's readiness for SARIMA application. The model was trained on the transformed data, and its performance was evaluated using metrics like RMSE and MAPE. The SARIMA model provided reliable forecasts, accounting for both seasonal and non-seasonal variations in ATM cash demand.          

### Prophet Model

The Prophet model, developed by Facebook, was selected for its flexibility and robustness in handling time series data with missing values and outliers. The model was trained on monthly aggregated data, incorporating seasonality and trend components. Prophet's ability to handle strong seasonal effects and holidays made it a valuable tool for predicting ATM cash demand. The forecast results included confidence intervals, providing a comprehensive view of expected future withdrawals. The model's performance was evaluated using metrics such as MAE, RMSE, MAPE, and R-squared.    

### ANN Model
The Artificial Neural Network (ANN) model was chosen based on its capability to learn complex patterns from data. ANNs consist of layers of interconnected neurons that adjust their weights and biases during training to minimize prediction errors. The ANN model was trained on the time series data, and forecasts were generated for the test period. The model's performance was evaluated using accuracy metrics such as RMSE and MAPE. The ANN model's ability to capture non-linear relationships and intricate patterns made it a powerful tool for forecasting ATM cash demand.  


## Model Performance Error Metrics (RMSE, MAPE)
Evaluating model performance is essential to determine the accuracy and reliability of the forecasts. Two key metrics used in this project are Root Mean Square Error (RMSE) and Mean Absolute Percentage Error (MAPE). RMSE measures the average magnitude of the forecast errors, providing a clear indication of the model's accuracy. MAPE expresses the forecast error as a percentage of the actual values, making it easier to interpret the model's performance in relative terms. These metrics were calculated for each model to compare their effectiveness in predicting ATM cash demand.       

### RMSE & MAPE Comparison

The RMSE and MAPE values for the SARIMA, Prophet, and ANN models were compared to identify the most accurate forecasting method. Bar plots were created to visualize the RMSE and MAPE values for each model, highlighting their performance differences. This comparison revealed that the ANN model had the lowest RMSE and MAPE values, indicating superior accuracy compared to the SARIMA and Prophet models. The visual representation of these metrics helped in making an informed decision about the best model for forecasting ATM cash demand.       

### Model Performance Error Metrics: Results    

The results of the model performance evaluation showed that the ANN model outperformed both the SARIMA and Prophet models in terms of RMSE and MAPE. The ANN model's ability to capture complex patterns and non-linear relationships in the data resulted in more accurate forecasts. The SARIMA and Prophet models, while effective in handling seasonality and trend components, exhibited higher error metrics, making them less reliable for this specific dataset. Based on these results, the ANN model was selected as the best option for forecasting ATM cash demand, ensuring robust and accurate predictions.       