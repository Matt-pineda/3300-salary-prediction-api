# 3300 - Salary Prediction Model API

💼 Salary Prediction API
This repository contains a machine learning-powered API that predicts salaries based on user-input features such as education, experience, and job-related data. Built as part of a personal project to deepen my skills in Python, scikit-learn, and API deployment, this tool demonstrates how data analytics and web services can be combined to deliver practical, real-time insights.

🚀 Project Overview
The goal of this project was to build a simple yet functional API capable of returning salary predictions based on structured input data. The API was trained on a cleaned dataset of job postings and salary information, using regression models to estimate outcomes.

🔧 Tech Stack
Python – Core programming language

Flask – Lightweight web framework for building the API

scikit-learn – Used for model training and prediction

Pandas & NumPy – Data processing and manipulation

Joblib – For saving and loading the trained model

GitHub + Git – Version control and repository hosting

📂 Repository Structure
bash
Copy code
├── app.py                  # Main Flask application
├── salary_predict_model.ml # Serialized machine learning model
├── requirements.txt        # Dependencies
├── README.md               # Project documentation
├── /templates              # HTML front-end (optional if applicable)
└── /static                 # Static files (CSS, JS) if needed
📈 How It Works
The user submits a JSON payload or form input with relevant job/employee features.

The Flask API processes the request and uses the pre-trained regression model to predict the salary.

The API returns a predicted salary value.

Example input:

json
Copy code
{
  "education_level": "Bachelor’s",
  "years_experience": 3,
  "job_title": "Data Analyst",
  "industry": "Finance",
  "location": "Chicago"
}
Example output:

json
Copy code
{
  "predicted_salary": 75600
}
🧪 Running Locally
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/salary-prediction-api.git
cd salary-prediction-api
Create a virtual environment and activate it:

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install dependencies:

nginx
Copy code
pip install -r requirements.txt
Run the API:

nginx
Copy code
python app.py
Visit http://127.0.0.1:5000/ to access the API locally.

✅ Future Improvements
Add a front-end interface for user-friendly interaction

Expand the dataset and retrain model for improved accuracy

Add logging and error handling

Deploy via Docker or a cloud platform





