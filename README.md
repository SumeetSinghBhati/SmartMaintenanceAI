# Smart Maintenance AI

<br>

Welcome to the **Smart Maintenance AI** project! This repository houses a machine learning model designed for **predictive maintenance**, leveraging the capabilities of **XGBoost** to classify different types of equipment failures based on operational data.

<br>

## Project Overview

In industries where machinery and equipment play critical roles, predicting failures before they occur can save significant costs and downtime. This project employs a **supervised learning** approach to classify the likelihood of equipment failure using sensor and operational data. The model processes features such as air temperature, process temperature, rotational speed, torque, and tool wear to predict various failure types.

<br>

## Key Features

- **Predictive Modeling:** Utilizes the **XGBoost** classifier to predict equipment failure types.<br>
- **Hyperparameter Tuning:** Implements **GridSearchCV** for hyperparameter optimization to enhance model performance.<br>
- **Feature Importance Visualization:** Analyzes and visualizes the importance of different features affecting model predictions.<br>
- **Robust Evaluation:** Evaluates the model's accuracy using various metrics, including the classification report.

<br>

## Dataset

The dataset used in this project is titled **Predictive Maintenance Dataset**, which contains operational data with the following key attributes:

<table>
  <tr>
    <th>Attribute</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>UDI</strong></td>
    <td>Unique device identifier.</td>
  </tr>
  <tr>
    <td><strong>Product ID</strong></td>
    <td>Identifier for the product.</td>
  </tr>
  <tr>
    <td><strong>Type</strong></td>
    <td>Type of the product (L, M, H).</td>
  </tr>
  <tr>
    <td><strong>Air temperature [K]</strong></td>
    <td>Air temperature in Kelvin.</td>
  </tr>
  <tr>
    <td><strong>Process temperature [K]</strong></td>
    <td>Process temperature in Kelvin.</td>
  </tr>
  <tr>
    <td><strong>Rotational speed [rpm]</strong></td>
    <td>Rotational speed in revolutions per minute.</td>
  </tr>
  <tr>
    <td><strong>Torque [Nm]</strong></td>
    <td>Torque applied in Newton-meters.</td>
  </tr>
  <tr>
    <td><strong>Tool wear [min]</strong></td>
    <td>Wear on the tool measured in minutes.</td>
  </tr>
  <tr>
    <td><strong>Target</strong></td>
    <td>Binary indicator of failure (1 for failure, 0 for no failure).</td>
  </tr>
  <tr>
    <td><strong>Failure Type</strong></td>
    <td>Class of failure (e.g., No Failure, Heat Dissipation Failure, etc.).</td>
  </tr>
</table>

<br>

## Model Performance

The model achieved an impressive **accuracy of 98.25%** on the test set. This high accuracy demonstrates the model's capability to effectively identify equipment failures and reduce unnecessary downtime. Here are some additional performance statistics:

- **Precision:** Measures the accuracy of the positive predictions. For instance, the precision for the "Heat Dissipation Failure" class is **95.0%**, indicating a high level of correctness in identifying true failures.<br>
- **Recall:** Represents the model's ability to capture all actual positive cases. The recall for the "No Failure" class is **97.8%**, ensuring that most non-failure cases are accurately classified.<br>
- **F1-Score:** This metric balances precision and recall. The F1-score for "Tool Wear Failure" stands at **93.5%**, reflecting a strong performance in identifying this type of failure without many false positives.

<br>

## Feature Importance

The model's feature importance indicates which variables are most influential in predicting failures, helping guide maintenance strategies and operational adjustments. For example, **rotational speed** and **tool wear** emerged as the top contributors to the model's predictions, suggesting that monitoring these metrics could significantly enhance maintenance efforts.

<br>

## Deployment

This project is deployed and accessible online at:  
<a href="https://huggingface.co/spaces/sumeetsinghbhati07/SmartMaintenanceAI?logs=container" target="_blank">Smart Maintenance AI on Hugging Face</a>

<br>

## Contributing

Contributions are welcome! If you would like to contribute, please fork the repository and submit a pull request.
