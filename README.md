# Bangladesh Weather Predictions 🌦️

A machine learning-based project to predict weather patterns in Bangladesh. This project leverages advanced techniques such as feature engineering, oversampling (SMOTE), and hyperparameter tuning to handle imbalanced datasets and achieve optimal predictions.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Future Improvements](#future-improvements)
- [Contact](#contact)

## Overview
Bangladesh experiences six distinct seasons, but with global warming, the weather is becoming increasingly unpredictable. This project aims to predict key weather attributes, such as rainfall and temperature, to aid in disaster management and agricultural planning. The project addresses challenges like non-linear patterns in weather data by using machine learning models like XGBoost, CatBoost, and LGBM.

## Features
- **Data Preprocessing**: Includes handling missing values, encoding categorical variables, and outlier detection.
- **Exploratory Data Analysis (EDA)**: Visualizations for temperature, rainfall, humidity, and wind speed distributions.
- **Oversampling with SMOTE**: Balances the dataset for better predictions.
- **Model Evaluation**: Tested models include Logistic Regression, Random Forest, Decision Tree, XGBoost, CatBoost, and LGBM.
- **Hyperparameter Tuning**: Optimized models using GridSearchCV for maximum accuracy.

## Technologies Used
- **Programming Languages**: Python
- **Libraries**:
  - Data Handling: `pandas`, `numpy`
  - Visualization: `matplotlib`, `seaborn`
  - Machine Learning: `scikit-learn`, `xgboost`, `catboost`, `lightgbm`, `imblearn`
  - API Deployment: `Flask`

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/MonirulIslamm08/Bangladesh_Weather_Predictions.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Prepare the dataset (`Weather_Data.csv`) and place it in the root directory.

## Usage
1. Run the Jupyter Notebook for EDA and preprocessing:
   ```bash
   jupyter notebook
   ```
2. Train the models:
   ```bash
   python train_models.py
   ```
3. Deploy the model as a Flask API:
   ```bash
   python app.py
   ```
4. Make predictions via the API:
   ```bash
   curl -X POST -H "Content-Type: application/json" -d '{"features": [20.7, 22.9, 19.5, 23.4, 10.6, ...]}' http://127.0.0.1:5000/predict
   ```

## Results
The models were evaluated on accuracy, precision, and recall. The best-performing models are:
- **XGBoost**: 88.2% accuracy
- **CatBoost**: 87.8% accuracy
- **LGBM**: 88.8% accuracy

## Future Improvements
- Integrate more advanced deep learning models for weather predictions.
- Expand the dataset with real-time weather data using APIs.
- Build a user-friendly web interface for non-technical users.

## Contact
- **LinkedIn**: [Monirul Islam](https://www.linkedin.com/in/monirul-m08/)
- **GitHub**: [MonirulIslamm08](https://github.com/MonirulIslamm08)
- **Email**: md08monirul@gmail.com
