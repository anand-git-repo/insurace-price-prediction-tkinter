#Insurance Price Prediction with tkinter 
This repository contains code for predicting insurance prices using machine learning. It includes data preprocessing, model training, model evaluation, and GUI implementation.

Data
The data used in this project is in the insurance.csv file, located in the root directory. It contains information about individuals and their insurance prices.

Preprocessing
The data is read using Pandas and then preprocessed. The sex column is converted to a numerical column, with 0 representing female and 1 representing male. The smoker column is also converted to a numerical column, with 1 representing yes and 0 representing no. The region column is converted to numerical values 1-4 corresponding to southwest, southeast, northwest, and northeast. Null values are checked and the data is described to gain insights about it.

Model Training
Four regression models are trained using Scikit-learn's LinearRegression, SVR, RandomForestRegressor, and GradientBoostingRegressor. The GradientBoostingRegressor model provides the best results.

Model Evaluation
The r2_score and mean_absolute_error metrics are used to evaluate the models' performance. The GradientBoostingRegressor model provides the highest r2_score and lowest mean_absolute_error.

GUI
A GUI is implemented using Tkinter, allowing users to input their details and get a predicted insurance price based on the trained GradientBoostingRegressor model.

Saving Model
The trained GradientBoostingRegressor model is saved using the joblib library, allowing it to be loaded and used for making predictions in other applications.

File Structure
The main files in this repository are:

insurance.csv: the data used in this project.
insurance_price_prediction.py: the Python script containing the code for preprocessing, training, and evaluating the models, as well as implementing the GUI.
gbr_model: the saved GradientBoostingRegressor model.
