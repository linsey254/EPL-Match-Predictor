# EPL Match Outcome Predictor

A machine learning-based project for predicting the outcomes of English Premier League (EPL) matches. Using match statistics such as shots, possession, fouls, yellow/red cards, and corners, this project predicts whether the home team will win, lose, or draw. The project is built with a Random Forest classifier and includes a command-line interface for prediction.

## Features
- Predicts EPL match outcomes based on match statistics
- Includes interactive input for team details and match statistics
- Uses a pre-trained Random Forest model for predictions
- Scaled data with StandardScaler for consistent input/output values

## Technologies Used
- Python
- Scikit-Learn (RandomForestClassifier, StandardScaler)
- Pandas
- Joblib for model saving/loading

## Getting Started

### Prerequisites
1. Install Python 3.x
2. Install necessary libraries:
    ```bash
    pip install pandas scikit-learn joblib
    ```

### Repository Structure
The project is organized as follows:

```plaintext
epl_match_outcome_predictor/
├── data/
│   ├── epl_dataset.csv         # Training dataset for EPL matches
├── models/
│   ├── best_rf_model.pkl       # Pre-trained Random Forest model
│   ├── scaler.pkl              # Scaler for input data
├── src/
│   ├── predict_match.py        # Main script for predicting match outcomes
│   ├── train_model.py          # Script to train the Random Forest model
│   ├── utils.py                # Utility functions for data processing and feature engineering
├── tests/
│   ├── test_predict_match.py   # Unit tests for the prediction functionality
│   ├── test_train_model.py     # Unit tests for model training functions
├── README.md                   # Project README file
├── requirements.txt            # List of dependencies for the project
