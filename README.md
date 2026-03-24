# Customer Churn Prediction using End-to-End ML Pipeline

## 📌 Project Objective
The goal of this project is to build a production-ready machine learning pipeline that predicts whether a customer will stop using a service (Churn). This project focuses on reusability and clean code practices using the Scikit-learn Pipeline API.

## 🛠️ Methodology & Approach
I implemented a structured approach to handle the Telco Churn dataset:
1. **Data Preprocessing:** Handled missing values and converted data types for analysis.
2. **Feature Engineering:** Used `ColumnTransformer` to automate:
   - **Scaling:** Applied `StandardScaler` to numerical features.
   - **Encoding:** Applied `OneHotEncoder` to categorical features.
3. **Model Selection:** Implemented `RandomForestClassifier` for robust predictions.
4. **Pipeline Construction:** Integrated preprocessing and classification into a single `Pipeline` object to prevent data leakage and ensure reproducibility.
5. **Model Persistence:** Exported the final trained model using `joblib` for easy deployment.

## 📊 Key Results
- **Automation:** The entire workflow from raw data to prediction is handled by a single pipeline.
- **Model Accuracy:** Achieved a competitive accuracy score on the test set.
- **Scalability:** The pipeline can be easily updated with different models or new data.

## 📁 Project Structure
- `Telco Customer.ipynb`: Complete development notebook with analysis and training.
- `churn_model_pipeline.pkl`: The serialized (saved) model ready for production.
- `README.md`: Project documentation.

## 🚀 Technologies Used
- Python
- Pandas & NumPy
- Scikit-learn (Pipeline, ColumnTransformer)
- Joblib (Model Serialization)
