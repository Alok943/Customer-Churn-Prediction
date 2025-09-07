Customer Churn Prediction for a Telecom Company

Project Overview

This project focuses on building a machine learning model to predict customer churn for a fictional telecom company. By identifying customers who are at high risk of leaving, the business can proactively engage them with targeted retention strategies. This project covers the complete machine learning pipeline from data exploration and preprocessing to model training, evaluation, and tuning.

Dataset

The dataset used is the Telco Customer Churn dataset, sourced from Kaggle. It contains customer account information, demographic data, and the services each customer has signed up for.

    Source: Kaggle Telco Customer Churn

Methodology

    Exploratory Data Analysis (EDA): Investigated the dataset to understand feature distributions and their relationships with the target variable (Churn).

    Data Preprocessing: Cleaned the data by handling missing values and converting categorical features into a numerical format using one-hot encoding. Numerical features were scaled using StandardScaler.

    Handling Class Imbalance: Addressed the imbalanced nature of the dataset using two techniques: class_weight='balanced' in the model parameters and the SMOTE (Synthetic Minority Over-sampling Technique).

    Model Building: Trained and evaluated several classification models:

        Logistic Regression

        Random Forest Classifier

    Hyperparameter Tuning: Utilized GridSearchCV to find the optimal hyperparameters for the best-performing model (Random Forest) to maximize its predictive performance.

Key Findings & Results

The project successfully developed a model capable of predicting customer churn with a focus on identifying at-risk customers.

    The final Tuned Random Forest model achieved a recall of 80% for the churn class, successfully identifying 8 out of 10 customers who would actually leave.

    Feature Importance Analysis revealed that the primary drivers of churn are:

        Contract Type (Month-to-month)

        Customer Tenure (how long they have been a customer)

        Monthly Charges

    The Default Random Forest model provided a more balanced performance with an overall accuracy of 80% and a precision of 61%.

Model Performance Comparison

The chart below compares the performance of the different models on the churn class (1).

(Here you would paste a screenshot of the model comparison plot you created)

Technologies Used

    Python

    Pandas & NumPy: for data manipulation

    Matplotlib & Seaborn: for data visualization

    Scikit-learn: for machine learning modeling, preprocessing, and evaluation

    Imbalanced-learn: for SMOTE

    Jupyter Notebook / Google Colab: as the development environment

How to Run This Project

    Clone this repository: git clone https://github.com/your-username/Customer-Churn-Prediction.git

    Navigate to the project directory: cd Customer-Churn-Prediction

    Install the required libraries: pip install -r requirements.txt

    Open and run the Jupyter Notebook file (.ipynb).
