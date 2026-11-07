California House Price Prediction 🏡

Project Overview

This project focuses on predicting median house values in California using Machine Learning regression algorithms.

The goal is to explore housing data, perform data preprocessing, train different regression models, and evaluate their predictive performance.

Dataset

* Dataset: California Housing Dataset
* Source: Scikit-learn
* Target Variable: MedHouseVal
* Task: Regression

The target represents median house values for geographic areas in California, measured in units of $100,000.

Technologies & Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Joblib
* Google Colab

Project Workflow

1. Data Loading and Exploration
2. Exploratory Data Analysis (EDA)
3. Data Quality Checks
4. Feature Selection and Target Definition
5. Train-Test Split
6. Feature Scaling for Linear Regression
7. Model Training
8. Model Evaluation
9. Feature Importance Analysis
10. Model Saving and Persistence

Machine Learning Models

Two main approaches were evaluated:

* Linear Regression
* Random Forest Regressor

An additional Random Forest model was trained with adjusted hyperparameters to investigate overfitting.

Model Performance

Model	MAE	RMSE	R² Score
Linear Regression	0.5332	0.7456	0.5758
Random Forest	0.3268	0.5040	0.8062
Tuned Random Forest	0.3309	0.5113	0.8005

Best Test Performance: Random Forest Regressor

* R² Score: 0.8062
* MAE: 0.3268
* RMSE: 0.5040

The original Random Forest model achieved the best test-set performance among the evaluated models.

Feature Importance

The Random Forest model identified the following important features:

* MedInc
* AveOccup
* Latitude
* Longitude
* HouseAge
* AveRooms
* Population
* AveBedrms

Permutation Importance was also used to investigate how individual features affect model performance on the test set.

Model Persistence

The trained Random Forest model was saved using Joblib:

* house_price_model.pkl
* feature_names.pkl

Project Structure

California-House-Price-Prediction/
│
├── house_price_prediction.ipynb
├── house_price_model.pkl
├── feature_names.pkl
├── README.md
└── .gitattributes

How to Run

1. Clone this repository.
2. Install the required Python libraries.
3. Open the Jupyter Notebook in Google Colab or Jupyter.
4. Run the notebook cells sequentially to reproduce the workflow and train the models.

Future Improvements

* Hyperparameter optimization using cross-validation.
* Further model evaluation and error analysis.
* Experimenting with additional regression algorithms.
* Building an interactive prediction application.

Author

Kamal2992005

GitHub: https://github.com/Kamal2992005

⸻

This project was developed as a practical Machine Learning learning project.
