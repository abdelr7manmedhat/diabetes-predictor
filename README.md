# Diabetes Prediction App

A simple Flask web app that predicts whether a person is likely to have diabetes based on health-related inputs. The app uses a Random Forest model trained on the Pima Indians Diabetes dataset.

---

## Dataset
The dataset used is named `kaggle_diabetes.csv`.

**Source**: Local file `kaggle_diabetes.csv`
- Features used:
  - Pregnancies
  - Glucose
  - Blood Pressure
  - Skin Thickness
  - Insulin
  - BMI
  - Diabetes Pedigree Function
  - Age

---

## How It Works

1. The model is trained using `train_model.py`
2. Model is saved as `diabetes_model.pkl`
3. The Flask app (`app.py`) loads the model and takes input from a web form.
4. The prediction is displayed on the result page.

---

## Installation and Running Locally

```bash
git clone https://github.com/abdelr7manmedhat/diabetes-predictor.git
cd diabetes-predictor
pip install -r requirements.txt
python train_model.py
python app.py
```

Visit `http://127.0.0.1:5000` in your browser.

---

## Project Structure

```
diabetes_app/
├── app.py
├── train_model.py
├── diabetes_model.pkl
├── kaggle_diabetes.csv
├── requirements.txt
├── Procfile
└── templates/
    └── index.html
```

---

## Deployment

This app can be deployed on platforms like **Heroku**, **Render**, etc.  
Already includes:
- `Procfile`
- `requirements.txt`
- `Flask` app structure

---

## Tech Stack

- Python
- Flask
- Scikit-learn
- Pandas
- HTML / Bootstrap

---

## Author

Developed by [Abdelrhman Medhat](https://github.com/abdelr7manmedhat)

---

## License

This project is for educational purposes.
