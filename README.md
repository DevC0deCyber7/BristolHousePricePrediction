# BristolHousePricePrediction
🏡 House Price Predictor
A machine learning project to predict house prices using CatBoost Regression. This project includes data preprocessing, model training, and evaluation and is built with MLOps best practices using DVC and Docker for versioning and reproducibility.

📌 Overview: Preprocessed housing data for feature engineering and cleaning.

Trained a CatBoost regression model to predict house prices.

Evaluated model performance using RMSE, R² score, and MAPE.

Utilised DVC for data and model version control.

Containerised the application using Docker for easy deployment and scalability.

Organised a modular codebase with separate scripts for ingestion, preprocessing, training, and evaluation.

🛠 Technologies Used: Python (Pandas, NumPy, CatBoost)

CatBoost Regression

Model Evaluation: RMSE, R² Score, MAPE

MLOps Tools: DVC (Data Version Control), Docker

FastAPI / Streamlit for deployment

📊 Model Evaluation: The model was evaluated using:

Root Mean Squared Error (RMSE)

R² Score

Mean Absolute Percentage Error (MAPE)

The CatBoost model provided strong predictive performance after proper data preprocessing.

📁 Evaluation scripts: src/model_evaluation.py

🚀 How to Run 1.⁠ ⁠Clone the repository:

git clone https://github.com/your-username/house-price-predictor.git cd house-price-predictor 2.⁠ ⁠Set up a virtual environment and install dependencies:

python -m venv venv pip install -r requirements.txt

3.⁠ ⁠Run DVC pipeline to pull data and model:

dvc pull dvc repro

4.⁠ ⁠Launch the app:

FastAPI:

uvicorn app.app: app --reload

Streamlit:

streamlit run app/main.py
