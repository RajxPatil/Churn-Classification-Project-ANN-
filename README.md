# Churn Classification Project

## Overview

This project is designed to predict customer churn using a dataset of customer attributes. By leveraging machine learning models, the project provides predictions about whether a customer is likely to churn. It includes data preprocessing, feature engineering, and training an artificial neural network (ANN).

## Features

- **Customer Attributes**: Includes features like Geography, Gender, Age, Balance, and more.
- **Data Preprocessing**: Encoding categorical data, scaling numerical features, and handling missing values.
- **Machine Learning Model**: Uses an Artificial Neural Network (ANN) for churn prediction.
- **Deployment**: Provides a Python application interface for predictions.

## Files in the Repository

- **Churn_Modelling.csv**: Dataset containing customer data.
- **app.py**: Streamlit app for user interaction and real-time predictions.
- **experiments.ipynb**: Jupyter Notebook containing exploratory data analysis (EDA) and model experimentation.
- **prediction.ipynb**: Notebook for testing and generating predictions.
- **model.h5**: Trained ANN model saved in HDF5 format.
- **Scalar.pkl**: Pickle file containing the fitted StandardScaler for numerical feature scaling.
- **Label_encoder_gender.pkl**: Pickle file containing the fitted LabelEncoder for the Gender column.
- **One_hot_encoder_geo.pkl**: Pickle file containing the fitted OneHotEncoder for the Geography column.
- **requirements.txt**: Lists the Python dependencies for this project.
- **logs/**: Directory containing logs for training and debugging.

## Setup and Installation

### Clone the Repository:

```bash
git clone <repository_url>
cd churn-classification
```

### Create and Activate a Virtual Environment:

```bash
python3 -m venv venv
source venv/bin/activate   # For Linux/Mac
venv\Scripts\activate    # For Windows
```

### Install Dependencies:

```bash
pip install -r requirements.txt
```

### Run the Application:

```bash
streamlit run app.py
```

## Dataset

The dataset contains the following key columns:

- **CustomerID**: Unique identifier for each customer.
- **Geography**: Country of residence (e.g., France, Germany, Spain).
- **Gender**: Male or Female.
- **Age**: Age of the customer.
- **Balance**: Bank balance of the customer.
- **Exited**: Target variable (1 = Churn, 0 = Not Churn).

## Model

The project uses an Artificial Neural Network (ANN) built with the following architecture:

- **Input layer**: Number of input neurons matches the number of features.
- **Hidden layers**: Two dense layers with ReLU activation.
- **Output layer**: Single neuron with sigmoid activation for binary classification.

## Results

- **Accuracy**: 90.36 % 

## Usage

To use the application:

1. Run the `app.py` file using Streamlit.
2. Enter the required customer details in the web interface.
3. Click on the "Predict" button to see whether the customer is likely to churn.

## Contributing

Feel free to fork this repository and submit pull requests. For significant changes, open an issue to discuss your ideas.
