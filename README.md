# 💡 LoyaltyLens: Customer Churn Prediction

**LoyaltyLens** is a machine learning-powered web application that predicts the likelihood of customer churn based on user-provided data. It utilizes a trained neural network model to analyze customer behavior patterns and generate churn predictions. 

The application features a clean and interactive **Streamlit interface**, along with **Jupyter notebooks** for model experimentation and reproducibility.

---

## 🚀 Features

- 🔍 **Customer Churn Prediction**  
  Predicts whether a customer is likely to churn using a trained ML model.

- 🖥️ **Streamlit Web Interface**  
  Simple and intuitive UI for entering customer data and viewing prediction results.

- ⚙️ **Data Preprocessing**  
  Includes numerical scaling, categorical encoding, and feature engineering.

- 🧪 **Model Experimentation**  
  Interactive Jupyter Notebooks (`experiments.ipynb`, `prediction.ipynb`) for training, evaluation, and predictions.

- 💾 **Model Persistence**  
  Saves trained model and preprocessing pipeline for reuse without retraining.

---

## 🧠 Model Details

- **Architecture**: A fully connected neural network built using **TensorFlow/Keras**.
- **Input Features**:
  - `CreditScore`
  - `Geography`
  - `Gender`
  - `Age`
  - `Tenure`
  - `Balance`
  - `NumOfProducts`
  - `HasCrCard`
  - `IsActiveMember`
  - `EstimatedSalary`

- **Preprocessing**:
  - **Scaling**: Numerical features are scaled using `StandardScaler`.
  - **Encoding**:
    - Categorical features like `Geography` → `OneHotEncoder`
    - Binary features like `Gender` → `LabelEncoder`

---

## 📦 Dependencies

```text
tensorflow==2.18.0
streamlit==1.42.1
scikit-learn==1.6.1
pandas==2.2.3
numpy==2.0.2

📲 Usage Instructions
# 1. Clone the repository
git clone https://github.com/your-username/LoyaltyLens.git
cd LoyaltyLens

# 2. Install dependencies using pipenv
pipenv install
pipenv shell

# (Alternatively, use pip if you prefer)
# pip install -r requirements.txt

# 3. Run the Streamlit web application
streamlit run app.py

# 4. Interact with the app
# - Enter customer details like Credit Score, Geography, Gender, Age, etc.
# - Click "Predict Churn"
# - View the model's prediction and churn probability

# 5. (Optional) Use Jupyter Notebooks for experimentation
# - Open 'experiments.ipynb' to train and evaluate models
# - Open 'prediction.ipynb' to test predictions on new data

📁 Project Structure
LoyaltyLens/
├── app.py                     # Streamlit application
├── experiments.ipynb          # Model training & evaluation
├── prediction.ipynb           # Making predictions
├── model/                     # Saved model & preprocessing pipeline
├── data/                      # Input data (raw/processed)
├── Pipfile                    # Pipenv environment definition
├── Pipfile.lock               # Locked versions of dependencies
└── README.md                  # Project documentation

