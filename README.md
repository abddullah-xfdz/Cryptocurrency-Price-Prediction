# Cryptocurrency Price Prediction

A machine learning project I built to predict cryptocurrency price movements using Python and XGBoost.

The goal was to predict whether the next recorded price would go up or down based on historical P2P exchange data.

## About the Project

I wanted to explore how machine learning could be used to analyze cryptocurrency markets and identify price movement patterns.

I worked with real exchange data, cleaned and prepared it, created new features, and trained an XGBoost classification model to predict price direction.

## What I Did

- Explored the dataset and handled missing or invalid values.
- Worked with historical cryptocurrency P2P exchange data.
- Created features from timestamps and pricing information.
- Prepared the data for machine learning.
- Split the dataset chronologically into training and testing sets.
- Trained an XGBoost classification model.
- Evaluated predictions using accuracy, precision, recall, F1-score, and a confusion matrix.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Jupyter Notebook

## Dataset

I used the P2P BOB Exchange dataset available on Kaggle.

[Dataset on Kaggle](https://www.kaggle.com/datasets/andreschirinos/p2p-bob-exchange)

## How It Works

1. Load the historical exchange dataset.
2. Clean the data and prepare the features.
3. Create labels based on whether the next recorded price increases.
4. Split the data into training and testing sets based on time.
5. Train the XGBoost model.
6. Evaluate its predictions on the test data.

## How to Run

1. Download or clone this repository.
2. Open `crypto_price_predication.ipynb` in Jupyter Notebook or Google Colab.
3. Install the required libraries:

   `pip install pandas numpy scikit-learn xgboost kagglehub pyarrow matplotlib`

4. Run the notebook cells in order.

The notebook can download the dataset using KaggleHub or read a local `dashboard_summary.parquet` file.

## What I Learned

This project helped me understand how important data preprocessing and feature engineering are in machine learning.

I also learned how to work with time-based datasets, avoid data leakage, and evaluate classification models using different metrics.

## Limitations

The model predicts the direction of the next recorded price, not the exact future cryptocurrency price.

It is a learning project and is not intended to provide financial or trading advice.
