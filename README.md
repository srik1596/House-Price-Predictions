Imported and loaded House Price Prediction dataset(train and test)
Imported necessary libraries
Handled missing values:
  - Numerical columns: filled with median.  
  - Categorical columns: filled with None
Separated the target SalePrice from train dataset columns.
Categorical features: applied One-Hot Encoding. 
Aligned train and test feature columns after encoding.
Done log transformation to the skewed numerical using np.log1p()
Also log-transformed SalePrice
Applied RandomForestregressor
Evaluated using RMSE on the log scale, then converted back to original scale to interpret actual error in SalePrice
Identified which features most influence the predictions from the trained Random Forest using .feature_importances_
Used the trained model to predict on the test dataset
Converted predictions back from log scale to original scale.
Saved submission file House_Price_Prediction.csv
