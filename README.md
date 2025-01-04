# ALHOZ_Homeworks_NIE-MVI

## Network Intrusion Detection

Download the dataset file: MachineLearningCSV.zip from:

https://drive.google.com/file/d/1BY4ZT0183EvloEvIwCVhF3d1voXfga6k/view?usp=drive_link

Place it in the project folder and unzip it

## Contributions

1. Correct Evaluation Metric
2. Adressing data imblance
3. Benchmark results for different ML models
4. Running code for training/evaluating



## Model Performance using K-Fold Cross-Validation

| Classifier                        | 5-Fold Balanced Accuracy |
| --------------------------------- | ------------------------ |
| Perceptron                        | 76.27                    |
| Neural Network with 3 dense layer | 85.73                    |
| Neural Network with 5 dense layer | 85.63                    |
| (1D-)CNN with 2conv 1fc layer     | 87.13                    |
| (1D-)CNN with 5conv layer         | 87.16                    |


### Perceptron

Please run the Perceptron.ipynb

### NN

Please run the NN.ipynb
There are two NN architectures:

1. 'nn3' - 3 layers
2. 'nn5' - 5 layers

### 1D-CNN

Please run the CNN.ipynb
There are two 1D-CNN architectures:

1. 'cnn2' - 2 conv layers
2. 'cnn5' - 5 conv layers
