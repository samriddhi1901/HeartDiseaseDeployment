# Heart Disease Prediction using Machine Learning

## Project Overview

This project predicts whether a patient is at risk of heart disease using Machine Learning. The model is trained using the Heart Disease dataset and deployed as a REST API using Flask.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Flask
- Joblib
- GitHub
- Render

## Machine Learning Model

- Algorithm: Random Forest Classifier
- Accuracy: 99%

## Project Structure

```
HeartDiseaseDeployment/
│── app.py
│── train_model.py
│── model.pkl
│── heart.csv
│── requirements.txt
│── README.md
```

## Installation

```bash
pip install -r requirements.txt
```

## Run the Application

```bash
python app.py
```

The API will run at:

```
http://127.0.0.1:5000
```

## API Endpoint

### POST /predict

Example JSON:

```json
{
  "age": 63,
  "sex": 1,
  "cp": 3,
  "trestbps": 145,
  "chol": 233,
  "fbs": 1,
  "restecg": 0,
  "thalach": 150,
  "exang": 0,
  "oldpeak": 2.3,
  "slope": 0,
  "ca": 0,
  "thal": 1
}
```

Example Response

```json
{
  "prediction": "Heart Disease Detected"
}
```

## Deployment

Render Deployment URL:
https://heartdiseasedeployment-b85c.onrender.com


