# Applied Long Short Term Memory to Air Quality UCI dataset

## Introduction:
The goal of this project is to implement an LSTM model to forecast CO(GT) levels in the Air Quality dataset obtained from the UCI machine learning repository. The model is trained using 3-fold cross-validation and the performance is evaluated using mean squared error (MSE), root mean squared error (RMSE), and mean absolute error (MAE).

## Methodology:
The dataset is split into training and test sets with 80% of the data used for training and the remaining 20% used for testing. The LSTM model is defined with a single LSTM layer with 64 units and a dense output layer. The model is compiled with mean squared error as the loss function and the Adam optimizer. The data is preprocessed by splitting it into sequences of 24 time steps and creating input/output pairs.

The model is trained using 3-fold cross-validation, where the data is split into 3 consecutive time periods. The model is trained on the first two time periods and validated on the third time period. The model is trained for 50 epochs with a batch size of 64. The performance of the model is evaluated on the validation set using MSE, RMSE, and MAE.

## Results:
The average performance of the LSTM model over 3-fold cross-validation is as follows:

Mean Squared Error (MSE): 0.3694
Root Mean Squared Error (RMSE): 0.6078
Mean Absolute Error (MAE): 0.4360

## Conclusion:
The LSTM model performed reasonably well in forecasting CO(GT) levels in the Air Quality dataset with an average RMSE of 0.6078. There is certainly room for improvement in the model's performance, but this serves as a good starting point for further experimentation and optimization.
