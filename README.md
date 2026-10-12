# 🔥 Forest Fire Weather Index (FWI) Prediction

A Machine Learning web application that predicts the **Forest Fire Weather Index (FWI)** based on weather conditions and fire-weather parameters using a trained ML model and Flask.

## 📌 Project Overview

Forest fires can cause significant damage to forests, wildlife, and the environment. This project uses machine learning to estimate the Forest Fire Weather Index based on input parameters such as temperature, relative humidity, wind speed, rainfall, and other fire-weather indicators.

The application provides a simple web interface where users enter the required values and receive a prediction.

## ✨ Features

- Predict FWI using a trained machine learning model.
- Simple and responsive web interface.
- Flask backend for handling user inputs and predictions.
- HTML and CSS for frontend design.
- Input validation using HTML form attributes.
- Easy to run locally.

## 🛠️ Tech Stack

- **Programming Language:** Python
- **Machine Learning:** Scikit-learn
- **Backend:** Flask
- **Frontend:** HTML, CSS
- **Data Processing:** NumPy, Pandas
- **Model Storage:** Pickle (if used in the project)

## 📂 Project Structure

```text
ml2/
│
├── templates/
│   ├── home.html
│   └── index.html
│
├── application.py
├── requirements.txt
├── README.md
│
├── models/                 # If applicable
│   ├── model.pkl
│   └── scaler.pkl
│
└── dataset/                # If applicable
    └── dataset.csv
```

*Note: Adjust the structure to match your actual project files.*

## 📊 Input Parameters

| Parameter | Description |
|---|---|
| Temperature | Ambient temperature |
| RH | Relative humidity |
| Ws | Wind speed |
| Rain | Rainfall |
| FFMC | Fine Fuel Moisture Code |
| DMC | Duff Moisture Code |
| ISI | Initial Spread Index |
| Classes | Encoded class feature, if required by the model |
| Region | Encoded region feature, if required by the model |

The input features and their order must match the features used during model training.

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd ml2
```

Replace `<YOUR_GITHUB_REPOSITORY_URL>` with your actual repository URL.

### 2. Create a virtual environment

**Windows:**

```powershell
python -m venv venv
```

Activate it:

```powershell
.\venv\Scripts\Activate.ps1
```

If PowerShell blocks activation, you can use Command Prompt:

```cmd
venv\Scripts\activate.bat
```

### 3. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Run the application

```bash
python application.py
```

### 5. Open in your browser

Visit:

```text
http://127.0.0.1:5000/
```

The application should now be available locally.

## 🚀 How to Use

1. Start the Flask application.
2. Open the application in your browser.
3. Enter the required weather and fire-related parameters.
4. Click **Predict FWI**.
5. View the predicted result.

## 🧠 Machine Learning Workflow

1. Collect and load the dataset.
2. Clean and preprocess the data.
3. Separate features and target values.
4. Split the dataset into training and testing sets.
5. Train and evaluate the machine learning model.
6. Save the trained model and any required preprocessing objects.
7. Load the saved objects in Flask.
8. Process user inputs and generate predictions.
9. Display the prediction on the web interface.

## 🔮 Future Improvements

- Add dropdown menus for categorical features.
- Improve input validation and error handling.
- Display prediction results with visual indicators.
- Evaluate the model using appropriate regression metrics.
- Deploy the application to a cloud platform.
- Improve accessibility and mobile responsiveness.

## ⚠️ Disclaimer

This application is intended for educational and experimental purposes. Predictions should not be treated as an official fire-risk assessment or used as the sole basis for emergency decisions.

## 👨‍💻 Author

**Shankar G L**

GitHub: [shankargl](https://github.com/shankargl)

---

⭐ If you find this project useful, consider giving the repository a star.