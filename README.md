📊 Customer Churn Prediction App

This project is an interactive Streamlit web application that predicts whether a telecom customer is likely to churn using a trained XGBoost Machine Learning model.
It allows users to input customer attributes, view churn probability, and visualize prediction confidence.

🚀 Features
🔍 Real-time Churn Prediction

Enter customer information and instantly get:

Churn vs. No-Churn prediction

Prediction confidence score

Risk level (Low / Medium / High)

Visual probability bar chart

🧠 Machine Learning Model

Model: XGBoost Classifier

Training Size: 7,043 telecom customers

Accuracy: ~77%

Techniques: Categorical encoding + SMOTE balancing

Features Used: 19 customer demographics, services, and account factors

🎨 Modern UI

Clean, responsive layout using Streamlit

Custom styling for prediction boxes

Side panel with model details and top predictors

📁 Project Structure
project/
│
├── churn_app.py                # main Streamlit application
├── customer_churn_model.pkl    # trained ML model
├── churn_encoders.pkl          # label encoders for categorical features
├── README.md                   # documentation
└── requirements.txt            # Python dependencies

🛠️ Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/your-repo/churn-prediction.git
cd churn-prediction

2️⃣ Install dependencies
pip install -r requirements.txt

3️⃣ Add Model Files

Ensure that the following files exist in the project directory:

customer_churn_model.pkl

churn_encoders.pkl

(Generate them in your notebook or training script before running the app.)

4️⃣ Run the Streamlit App
streamlit run churn_app.py

🧩 How It Works

User inputs customer attributes such as:

Demographics (gender, senior citizen, dependents…)

Subscribed services (Internet, backup, streaming…)

Account info (contract type, monthly charges, tenure…)

App preprocesses the data:

Converts binary fields to numerical values

Applies label encoders for categorical variables

The trained XGBoost model predicts:

Churn (1) or Not Churn (0)

Probability of each class

App displays:

Color-coded prediction box

Confidence percentage

Risk level

Probability bar chart

📈 Top Factors Affecting Churn

According to model importance:

Contract type

Tenure

Monthly Charges

Internet service type

Payment method

🧰 Technologies Used

Python

Streamlit

Scikit-learn

XGBoost

Pandas

Plotly

Joblib

📝 Future Improvements

Add SHAP explainability plots

Deploy using Streamlit Cloud / Docker

Add customer segmentation analytics

Improve model accuracy with feature engineering
