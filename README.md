# tripfare-ML-project
🚕 Trip Fare: Predicting Urban Taxi Fare with Machine Learning
This project aims to accurately predict taxi fares in urban environments using machine learning techniques, leveraging a rich dataset of historical taxi trips. The workflow covers the entire data science pipeline: from data loading and cleaning, through feature engineering and exploratory data analysis (EDA), to model building, evaluation, and deployment with a user-friendly Streamlit app.

Project Highlights
Data Understanding:
Loaded and explored a real-world taxi trip dataset, checking for missing values, duplicates, and data types to ensure data quality.

Feature Engineering:
Created insightful features such as trip distance (using the Haversine formula), time-of-day indicators (AM/PM, night flag), weekday/weekend flags, and converted timestamps to local time (EDT). These features help capture patterns like rush hours, night rides, and weekend effects on fare prices.

Exploratory Data Analysis (EDA):
Visualized and analyzed relationships between fare, distance, passenger count, time, and more. Identified outliers and trends, such as peak demand hours and fare distributions across different periods.

Data Transformation:
Handled outliers, fixed skewness in continuous variables, and encoded categorical variables to prepare the data for modeling.

Feature Selection:
Applied correlation analysis and model-based feature importance to select the most relevant predictors for fare estimation.

Model Building & Evaluation:
Trained and compared multiple regression models, including Linear Regression, Ridge, Lasso, Random Forest, and Gradient Boosting. Models were evaluated using R², MSE, RMSE, and MAE. Hyperparameter tuning was performed to optimize performance.

Deployment:
The best-performing model was saved and integrated into a Streamlit web application. Users can input trip details (locations, time, passenger count, etc.) and receive an instant fare prediction.

How to Use
Clone the repository and install requirements

Run the Streamlit app:

text
streamlit run app.py
Input trip details in the UI and get your fare prediction!

Key Learnings
Importance of geospatial and temporal features in fare prediction

Handling real-world data issues (missing values, outliers, skewness)

Model selection and hyperparameter tuning for regression tasks

Building interactive machine learning applications for end-users
