# NO2 Concentration Estimation using Machine Learning
This project aims to estimate surface NO2 (Nitrogen Dioxide) concentrations using Machine Learning. This is a cost-effective alternative to expensive physical air quality sensors.

# Concept
# The project uses satellite data (Remote Sensing) and ground-truth data to build a model that can predict air pollution levels. Instead of relying only on expensive sensors, we use:

Satellite Data: Sentinel-5P TROPOMI (NO2 columns), CHIRPS (Precipitation), and NOAA (Surface Temperature).
Ground Data: Real measurements from air quality stations in Lombardy and Veneto, Italy.
Models Compared
# I implemented and compared multiple machine learning algorithms to find the most accurate one:

Linear Regression: A baseline model.
Random Forest: For handling complex data relationships.
SVM (Support Vector Machine): Using RBF and Poly kernels for high-dimensional analysis.
Results Summary
# The models were evaluated using MAPE, MAE, and RMSE metrics. Based on the analysis:

SVM with Poly Kernel showed strong performance with a mean MAE of 0.164.
Random Forest also provided reliable estimations with a mean MAE of 0.185.
# Files inside
main.ipynb: Full pipeline including data loading, scaling (MinMaxScaler), model training, and cross-validation.
Train.csv: Contains the dataset with Latitude, Longitude, Precipitation, LST, and NO2 satellite readings.
