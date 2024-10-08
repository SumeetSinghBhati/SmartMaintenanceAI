Smart Maintenance AI
Welcome to the Smart Maintenance AI project! This repository houses a machine learning model designed for predictive maintenance, leveraging the capabilities of XGBoost to classify different types of equipment failures based on operational data.

Project Overview
In industries where machinery and equipment play critical roles, predicting failures before they occur can save significant costs and downtime. This project employs a supervised learning approach to classify the likelihood of equipment failure using sensor and operational data. The model processes features such as air temperature, process temperature, rotational speed, torque, and tool wear to predict various failure types.

Key Features
Predictive Modeling: Utilizes the XGBoost classifier to predict equipment failure types.
Hyperparameter Tuning: Implements GridSearchCV for hyperparameter optimization to enhance model performance.
Feature Importance Visualization: Analyzes and visualizes the importance of different features affecting model predictions.
Robust Evaluation: Evaluates the model's accuracy using various metrics, including classification report.
Dataset
The dataset used in this project is titled Predictive Maintenance Dataset, which contains operational data with the following key attributes:

UDI: Unique device identifier.
Product ID: Identifier for the product.
Type: Type of the product (L, M, H).
Air temperature [K]: Air temperature in Kelvin.
Process temperature [K]: Process temperature in Kelvin.
Rotational speed [rpm]: Rotational speed in revolutions per minute.
Torque [Nm]: Torque applied in Newton-meters.
Tool wear [min]: Wear on the tool measured in minutes.
Target: Binary indicator of failure (1 for failure, 0 for no failure).
Failure Type: Class of failure (e.g., No Failure, Heat Dissipation Failure, etc.).
Model Performance
The model achieved an impressive accuracy of 98.25% on the test set. This high accuracy demonstrates the model's capability to effectively identify equipment failures and reduce unnecessary downtime. Here are some additional performance statistics:

Precision: Measures the accuracy of the positive predictions. For instance, the precision for the "Heat Dissipation Failure" class is 95.0%, indicating a high level of correctness in identifying true failures.
Recall: Represents the model's ability to capture all actual positive cases. The recall for the "No Failure" class is 97.8%, ensuring that most non-failure cases are accurately classified.
F1-Score: This metric balances precision and recall. The F1-score for "Tool Wear Failure" stands at 93.5%, reflecting a strong performance in identifying this type of failure without many false positives.
Feature Importance
The model's feature importance indicates which variables are most influential in predicting failures, helping guide maintenance strategies and operational adjustments. For example, rotational speed and tool wear emerged as the top contributors to the model's predictions, suggesting that monitoring these metrics could significantly enhance maintenance efforts.

Deployment
This project is deployed and accessible online at:

Smart Maintenance AI on Hugging Face

Contributing
Contributions are welcome! If you would like to contribute, please fork the repository and submit a pull request.

License
This project is licensed under the MIT License - see the LICENSE file for details.
