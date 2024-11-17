Customer Churn Prediction with Deep Learning
This repository contains a comprehensive project aimed at predicting customer churn using deep learning techniques.
Churn prediction helps businesses identify customers likely to discontinue their services, enabling proactive measures to retain them.

Dataset
The project uses a Customer Churn Dataset, which includes demographic, usage, and account-related information about customers. Each record indicates whether the customer has churned (1) or not (0).

Dataset Overview
Total rows: 7043
Columns: 21
Target variable: Churn (the outcome you want to predict)

Data types:
Categorical: 18 columns (gender, Partner, Dependents, PhoneService, MultipleLines, etc.)
Numerical: 2 columns (tenure, MonthlyCharges).
Mixed types: TotalCharges is an object (which likely needs conversion).

Deep Learning Workflow

Data Preprocessing:
Handle missing values.
Encode categorical features using one-hot encoding.
Scale numerical features for better model performance.

Model Architecture:
A fully connected feedforward neural network (Multilayer Perceptron).

Layers:
Input layer: Matches the number of features.
Hidden layers: Multiple layers with ReLU activation for non-linearity.
Output layer: A single neuron with a sigmoid activation for binary classification.

Model Training:
Loss Function: Binary Crossentropy.
Optimizer: Adam for adaptive learning rate.
Evaluation Metrics: Accuracy, Precision, Recall, F1-score, and AUC.

Evaluation:
Split the dataset into training, validation, and test sets.
Monitor validation metrics to prevent overfitting.
Visualize learning curves (loss and accuracy).

Acknowledgments
Dataset: Publicly available customer churn datasets.
Libraries: TensorFlow, Keras, Pandas, NumPy, Matplotlib.


