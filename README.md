<p align="center"> 
# ABSTRACT
</p>

My project involved developing a machine learning model that predicted the alcohol content of wine using 11 features: density, residual sugar, fixed acidity, chlorides, pH, quality, sulphates, volatile acidity, citric acid, total sulfur dioxide, and free sulfur dioxide. My chosen performance metric I used for evaluation of my models was root mean squared error (RMSE). I performed 4 experiments and labelled the models model1, model2, model3, model4, and model5. Model1 was based on the original dataset with duplicate data. Model 2 was based on the data with duplicates dropped. Model3 was based on 2 normalized columns "free sulfur dioxide and total sulfur dioxide". Model4 was based on the normalized data with duplicates removed. Model5 was based on Model 4, but with feature selection (taking the most important features) turned on. My final chosen model was Model 4, a Catboost regressor model. My final chosen TUNED Model4 had the following performance metrics for predictions on the test sets: MAE = 0.2553, MSE = 0.1223, RMSE = 0.3497, R2 = 0.9172,  RMSLE = 0.0303, MAPE = 0.0243. For the same model, my final performance metrics for training were MAE = 0.2847, MSE = 0.1356, RMSE = 0.3675, R2 = 0.9079, RMSLE = 0.0316, MAPE = 0.0270. The RMSE = 0.3497 was good considering the alcohol content range on the original dataset was from 8.0 to 14.2. 

I also performed a regression analysis of my target variable "alcohol" against the most important feature, "density", at the end of the Google Colab notebook. The RMSE score for the predictions on the test data was RMSE = 0.7. This RMSE value was quite decent considering the alcohol content range on the original dataset was from 8.0 to 14.2. This would reinforce the finding that density was the most important feature from the generated feature importance table, suggesting density was a good predictor of alcohol content.

Here is my Youtube video on my project:
https://youtu.be/Y92-n7hZjko

Here is the UC Irvine dataset on wine quality I used:
https://archive.ics.uci.edu/dataset/186/wine+quality
