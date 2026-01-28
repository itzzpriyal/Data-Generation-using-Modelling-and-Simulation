# Data-Generation-using-Modelling-and-Simulation
This project models urban flooding using a rainfall–runoff simulation to generate synthetic data. Around 1000 rainfall scenarios were simulated by varying rainfall intensity, duration, drainage capacity, and soil absorption. The generated dataset was used to train and compare multiple ML regression models,with Random Forest giving the best results.
# Urban Flood Risk Simulation for Machine Learning

## Objective
- To model an urban flooding system using simulation
- To generate synthetic data through random environmental parameters
- To apply machine learning models on simulated data
- To compare model performance and identify the best model

## Simulation Methodology
The simulation models urban flooding based on the following parameters:
- Rainfall Intensity (mm/hr)
- Rainfall Duration (hours)
- Drainage Capacity (mm/hr)
- Soil Absorption (%)

Flood depth is calculated as excess water remaining after drainage and soil absorption. Random values within realistic bounds are used to simulate different rainfall scenarios.

## Dataset Generation
A total of 1000 simulation runs were performed.  
Each simulation produces a flood depth value, creating a dataset suitable for machine learning.

- Input features: rainfall and drainage parameters  
- Output target: flood depth (cm)

The flood depth distribution is positively skewed, reflecting real-world flood behavior where severe events are rare.

## Machine Learning Models Used
The following regression models were trained and evaluated:
- Linear Regression
- Ridge Regression
- Lasso Regression
- Decision Tree Regressor
- Random Forest Regressor
- Support Vector Regressor (SVR)
- K-Nearest Neighbors (KNN)

## Evaluation Metrics
Model performance was evaluated using:
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

Random Forest Regressor achieved the best performance due to its ability to capture nonlinear relationships.

## Tools and Technologies
- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab

## Repository Structure
Urban-Flood-Simulation-ML
┣ flood_simulation.ipynb
┣ README.md
┣ requirements.txt


## Conclusion
This project highlights how simulation-based data generation can be effectively used for machine learning when real-world data is limited. The integration of modelling, simulation, and ML provides a reliable approach for predicting flood severity in urban environments.

