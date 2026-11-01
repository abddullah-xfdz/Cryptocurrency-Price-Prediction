
Credit Card Fraud Detection

A machine learning project I built to detect potentially fraudulent credit card transactions using a neural network.

The main challenge in this project is the imbalanced dataset: fraud cases are much rarer than normal transactions. I focused on preparing the data carefully, training a model that pays attention to the minority class, and evaluating its predictions with the right metrics.
What I did

    Explored the transaction data and checked for missing values.
    Created additional features from transaction amount and elapsed time.
    Split the dataset into training, validation, and test sets.
    Standardized the features using statistics from the training data only.
    Built a neural network with TensorFlow/Keras and used class weights and focal loss to help with class imbalance.
    Selected the classification threshold on the validation set and evaluated the final model on a separate test set.

Tools and libraries

    Python
    Pandas and NumPy
    Scikit-learn
    TensorFlow / Keras
    Matplotlib
    KaggleHub (to download the dataset)

Dataset

I used the public, anonymized Credit Card Fraud Detection dataset, which contains transactions labeled as legitimate (0) or fraudulent (1). The dataset file is not included in this repository.
How to run

    Download credit_card_fraud_detection_FIXED.ipynb or open it in Google Colab / Jupyter Notebook.

    Install the dependencies if needed:
    pip install pandas numpy scikit-learn tensorflow kagglehub matplotlib

    Run the notebook from top to bottom. It will use creditcard.csv in the working directory if available; otherwise, it will try to download the dataset with KaggleHub (internet access required).

    Check the classification report, confusion matrix, fraud precision, recall, F1-score, and PR-AUC printed at the end.

Notes

Fraud detection is not just about overall accuracy, because a model can predict most transactions as legitimate and still appear highly accurate. That's why I focused on precision, recall, F1-score, and PR-AUC.

The notebook is a learning project, not a production fraud detection system. I haven't included final performance numbers here until the notebook has been run and verified on the complete dataset.
