# Rain Prediction Using Artificial Neural Network (ANN)

## Overview

This project builds a rain prediction model using an Artificial Neural Network (ANN) on the Australian weather dataset. The objective is to predict whether it will rain the following day (`RainTomorrow`) based on historical weather observations.

The project covers the complete machine learning workflow, including data preprocessing, missing value handling, feature encoding, feature scaling, model development, training, and evaluation.

---

## Dataset

**Dataset:** `weatherAUS.csv`

The dataset contains daily weather observations collected from multiple locations across Australia.

**Target Variable:**
- `RainTomorrow`
  - Yes → Rain expected the next day
  - No → No rain expected

---

## Features

The dataset contains weather-related features such as:

- MinTemp
- MaxTemp
- Rainfall
- Evaporation
- Sunshine
- WindGustDir
- WindGustSpeed
- WindDir9am
- WindDir3pm
- WindSpeed9am
- WindSpeed3pm
- Humidity9am
- Humidity3pm
- Pressure9am
- Pressure3pm
- Cloud9am
- Cloud3pm
- Temp9am
- Temp3pm
- RainToday
- Location
- Date
- and several additional weather attributes.

---

## Data Preprocessing

The following preprocessing steps were performed:

- Missing value handling
  - Mean imputation
  - Median imputation
  - Mode imputation
- Duplicate value checking
- Ordinal encoding for categorical features
- Label encoding for the target variable
- Standard scaling for numerical features
- Train-test splitting

---

## Model Architecture

The model was built using Keras Sequential API.

Architecture:

- Input Layer
- Dense Layer (ReLU)
- Dropout
- Dense Layer (ReLU)
- Dropout
- Dense Layer (ReLU)
- Dropout
- Flatten Layer
- Dense Layer (ReLU)
- Dropout
- Output Layer (Sigmoid)

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- TensorFlow / Keras

---

## Libraries

```python
pandas
matplotlib
scikit-learn
tensorflow
keras
numpy
```

Install dependencies:

```bash
pip install pandas matplotlib scikit-learn tensorflow
```

---

## Project Workflow

1. Load the dataset
2. Explore the data
3. Handle missing values
4. Encode categorical variables
5. Scale numerical features
6. Split data into training and testing sets
7. Build the ANN model
8. Train the model
9. Evaluate model performance
10. Predict rainfall

---

## Model Training

- Optimizer: Adam
- Loss Function: Binary Crossentropy
- Metric: Accuracy
- Epochs: 50
- Batch Size: 20
- Validation Split: 20%

---

## Repository Structure

```
Rain-Prediction/
│
├── rain_prediction.ipynb
├── weatherAUS.csv
├── README.md
└── requirements.txt
```

---

## Future Improvements

- Hyperparameter tuning
- Cross-validation
- Feature engineering
- Compare ANN with traditional machine learning models
- Model deployment using Flask or FastAPI
- Interactive prediction web application

---

## Results

The notebook demonstrates the complete implementation of an ANN-based binary classification model for rainfall prediction. Performance can be further improved through feature engineering, model tuning, and additional experimentation.

---

## Author

**Fahim Sami**

Machine Learning and Data Analytics Enthusiast

GitHub: https://github.com/samifahim07
