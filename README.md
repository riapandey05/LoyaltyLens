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
CreditScore,
Geography,
Gender,
Age,
Tenure,
Balance,
NumOfProducts,
HasCrCard,
IsActiveMember,
EstimatedSalary,
Preprocessing:Features are scaled using StandardScaler.
Categorical features are encoded using OneHotEncoder and LabelEncoder.

Dependencies
Key dependencies include:

tensorflow==2.18.0
streamlit==1.42.1
scikit-learn==1.6.1
pandas==2.2.3
numpy==2.0.2

## Usage
Streamlit App
Launch the app using the command above.
Enter customer details such as Credit Score, Geography, Gender, etc.
Click the "Predict Churn" button to view the prediction and churn probability.
Jupyter Notebooks
Use experiments.ipynb for training and evaluating models.
Use prediction.ipynb for making predictions on new data.

---

## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/LoyaltyLens.git
   cd LoyaltyLens

2. **Install Dependencies:**
    Use pipenv:
       pipenv install
       pipenv shell

3. **Run the Application:**
   streamlit run app.py


