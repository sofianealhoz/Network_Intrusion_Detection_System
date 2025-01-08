# ALHOZ_Homeworks_NIE-MVI

## Network Intrusion Detection

My blog-post about this project: https://medium.com/@sofiane.alhoz/network-intrusion-detection-22607082d4b2

## Introduction

This project aims to implement and evaluate the accuracy of different machine learning models for network flow classification in an Intrusion Detection System (NIDS).

Models tested: 
- **Perceptron**
- **NN3**
- **NN5**
- **CNN2**
- **CNN5**


I used K-Fold Cross-Validation to assess model performance and fine-tune hyperparameters.

## File Structure

📜 `models.py` → Defines the Perceptron, CNN, and Neural Network models  
📜 `preprocessing.py` → Handles data preprocessing (normalization, balancing, etc.)  
📓 `cnn.ipynb` → Training and evaluation of CNN models  
📓 `nn.ipynb` → Training and evaluation of Neural Networks  
📓 `perceptron.ipynb` → Training and evaluation of Perceptron model  
📓 `kfold_eval.ipynb` → Performs K-Fold Cross-Validation  
📁 `MachineLearningCVE` → Folder containing the dataset files 


## Installation & Requirements

📌 **Required Environment**  
- Python **3.8+**  
- Required libraries:  
  ```bash
  pip install torch scikit-learn numpy pandas matplotlib tensorboard enum34

Download the dataset file: MachineLearningCSV.zip from:

https://drive.google.com/file/d/1BY4ZT0183EvloEvIwCVhF3d1voXfga6k/view?usp=drive_link

Place it in the project folder and unzip it, then you should have the MachineLearningCVE in your file structure

## Hyperparameter Tuning

It is performed individually for each model within its respective `.ipynb` file.  
In the appropriate cell put the hyperparameters you want to test:


learning_rates = [1e-4, 1e-2, 1e-0]  
regularizations = [1e-6, 1e-4, 1e-2]

Then if you run the notebook you will get the best hyperparameters within that range and a plot that represent it.


## Model Performance using K-Fold Cross-Validation
It is performed in the KFold-eval.ipynb file.
There is a cell for each model that performs K-Fold evaluation, specifically five-fold evaluation in our case.

Specify the hyperparameters that you determined during the tuning process in the K-Fold function within the cell, then you will obtain the results as cell outputs: the balanced test acc for each fold, as well as the final 5-Fold Accuracy.


This is an exemple of results I finaly got:

| Classifier                        | 5-Fold Balanced Accuracy |
| --------------------------------- | ------------------------ |
| Perceptron                        | 76.27                    |
| Neural Network with 3 dense layer | 85.73                    |
| Neural Network with 5 dense layer | 85.61                    |
| (1D-)CNN with 2conv layer         | 88.14                    |
| (1D-)CNN with 5conv layer         | 88.18                    |
