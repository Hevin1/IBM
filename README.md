# Credit Card Fraud Detection Model Deployment in IBM Cloud
This project involves deploying a credit card fraud detection model using the Credit Card Fraud Detection dataset from Kaggle and a Random Classifier model in scikit-learn. The model is deployed on IBM Cloud using Watson Studio, and you can access it via an API endpoint.

# Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Model](#model)
- [Deployment Steps](#deployment-steps)
- [usage sample](#Sample-code-to-access-the-deployed-model)


## Introduction
The purpose of this project is to demonstrate how to deploy a machine learning model for credit card fraud detection in the cloud, making it accessible via an API endpoint. This README provides a step-by-step guide to replicate the deployment process.

## Dataset
The dataset used for this project is the "Credit Card Fraud Detection" dataset from Kaggle. You can find and download the dataset from [Kaggle]([https://www.kaggle.com/datasets](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)).

## Model
The machine learning model used for fraud detection is a Random Classifier model, created using scikit-learn.

## Deployment Steps
1. Create a Jupyter Notebook in Watson Studio:
   - Use IBM Watson Studio to create a Jupyter Notebook for your project.
2. Add the Dataset:
   - Upload and add the Credit Card Fraud Detection dataset to your project in Watson Studio.
3. Dataset Preprocessing:
   - Perform data preprocessing on the dataset to prepare it for training.
4. Understanding the Dataset:
   - Explore and analyze the dataset to gain insights into the data.
5. Data Visualization:
   - Create visualizations to better understand the data distribution.
6. Split the Dataset:
   - Split the dataset into training and testing subsets.
7. Model Training:
   - Train the Random Classifier model on the training data.
8. Model Testing and Evaluation:
   - Test the model on the test data and evaluate its performance.
9. Create Deployment Space in IBM Cloud:
   - Set up a deployment space in IBM Cloud for deploying your model.
10. Store the Model in the Deployment Space:
    - Store the trained model in the created deployment space.
11. Deploy the Model:
    - Deploy the model in the IBM Cloud environment.
12. Access the Model via API Endpoint:
    - After deployment, you will receive an API endpoint that can be used to access the model for real-time predictions.

# Sample code to access the deployed model
```python

import requests

url = "YOUR_API_ENDPOINT"
data = {
    # Input data for prediction
}

response = requests.post(url, json=data)
result = response.json()
print(result)
