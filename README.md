# Network Intrusion Detection System

Machine learning intrusion detection on network traffic. Several classifiers
are compared and evaluated with K-Fold cross validation.

## Models

Perceptron, fully connected neural networks (NN), and convolutional neural
networks (CNN), implemented in PyTorch.

## Stack

- Python 3
- PyTorch (models, training)
- scikit-learn (metrics, cross validation)
- pandas, NumPy (preprocessing)
- Jupyter Notebook (experiments)

## Structure

- `Semestral_Project/preprocessing.py` : data preparation.
- `Semestral_Project/models.py` : model definitions.
- `Semestral_Project/*.ipynb` : experiments and K-Fold evaluation.
- `Semestral_Project/MachineLearningCVE/` : dataset location.

## Dataset

CIC-IDS style flow data (MachineLearningCVE). The dataset is not versioned.
Place the files in `Semestral_Project/MachineLearningCVE/` before running.

## Usage

Open the notebooks under `Semestral_Project/` with Jupyter, or run the
preprocessing and training scripts directly.
