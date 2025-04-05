# LoyaltyLens: Customer Churn Prediction

LoyaltyLens is a machine learning-based application designed to predict customer churn.It leverages a trained neural network model to analyze customer data and determine the likelihood of churn.
The project includes a web-based interface built with Streamlit for user interaction and a Jupyter Notebook for experimentation and predictions.

## Features
- **Customer Churn Prediction**: Predicts the likelihood of a customer leaving based on input data.
- **Streamlit Web Interface**: User-friendly interface for entering customer data and viewing predictions.
- **Data Preprocessing**: Includes scaling, encoding, and feature engineering.
- **Experimentation**: Jupyter Notebook for model training, evaluation, and experimentation.
- **Model Persistence**: Trained model and preprocessing objects are saved and reused for predictions.

## Model Details
Architecture: The model is a neural network built using TensorFlow/Keras.
Input Features:
CreditScore
Geography
Gender
Age
Tenure
Balance
NumOfProducts
HasCrCard
IsActiveMember
EstimatedSalary
Preprocessing:Features are scaled using StandardScaler.
Categorical features are encoded using OneHotEncoder and LabelEncoder.


