# KC_houses-Regression-prediction

Comparing different regression models for predicting the house prices given the kc-houses dataset from https://www.kaggle.com/shivachandel/kc-house-data. 

The first model, a simple linear regression model is underfitting the model giving as a result a very poor R2 value as well as high mean_squared_error and mean_absolute_error values.

The second model, sklearn random forest regression model, is significantly improved and has an acceptable R2 value. The low and acceptable values for the mean_squared_error and mean_absolute_error also indicate that the model is probably not overfitting, as it often happens with decision trees.

The third model uses an sklearn multilayer perceptron with four layers of 256 nodes each. The model's metrics are a a bit worse than the random forest, indicating a 
weaker model.

The fourth and final model is a keras deep learning network with 5 layers and the number of nodes chosen so that overfitting can be avoided without the use of 
dropout layers. The model is trained for 200 epochs with an early stopping callback monitoring the mean absolute error. In the end we can see that the metrics of the model are still not better than the random forest regression model.
