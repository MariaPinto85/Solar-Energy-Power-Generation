# Solar-Energy-Power-Generation


This repository contains a comprehensive approach to forecasting solar energy generation using environmental and meteorological data. The project employs various machine learning techniques to predict solar power output based on key weather conditions, enhancing our understanding of how these factors influence photovoltaic (PV) power generation.

## Dataset

The dataset used for this project is the Solar Energy Power Generation Dataset from Kaggle. It includes 4,213 observations and 21 variables, capturing essential data for solar power analysis:

Variables: Temperature, humidity, cloud cover (high, medium, low), solar radiation, wind speed, and direction, among others.
New Features:
temp_humidity_index: Combines temperature and humidity for a measure of perceived warmth.
effective_solar_radiation: Adjusts solar radiation by cloud cover to estimate the actual energy reaching the panels.
total_cloud_cover: Aggregates cloud cover across multiple atmospheric layers.

## Project Workflow

Data Preprocessing: Cleaning, handling null values, and identifying outliers to ensure data quality.
Feature Engineering: Creating new features like temp_humidity_index and effective_solar_radiation to improve model accuracy.
Exploratory Data Analysis (EDA): Visualizing relationships between variables, such as solar radiation and cloud cover, and their impact on power generation.

## Model Development:
Algorithms Used: Random Forest Regressor, Gradient Boosting Regressor, and XGBoost Regressor.
Hyperparameter Tuning: Grid and Randomized Search for optimizing model parameters to achieve the best results.
Model Evaluation: Evaluated using Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE). Gradient Boosting showed the best RMSE, indicating good generalization on unseen data.
Key Results

Model Performance:
Random Forest: MAE = 254.8, RMSE = 406.8
Gradient Boosting: MAE = 257.1, RMSE = 398.1
XGBoost: MAE = 256.5, RMSE = 401.8
Feature Importance: Analysis showed that angle_of_incidence, zenith, azimuth, and cloud cover-related features are the most influential on solar power output.
Usage

Installation: Clone the repository and install required packages.
git clone https://github.com/MariaPinto85/Solar-Energy-Power-Generation.git
cd Solar-Energy-Power-Generation
pip install -r requirements.txt
Run the Analysis: Load the dataset, preprocess the data, and run the models by following the Jupyter notebook provided in the repository.
Customizable Parameters: Modify model parameters or try different features in the notebook to experiment with different forecasting results.
Future Work

## Further improvements can be made by:

Exploring additional machine learning algorithms.
Incorporating more advanced feature engineering techniques.
Applying deep learning models for potential performance enhancements.
License

This project is licensed under the MIT License - see the LICENSE file for details.

