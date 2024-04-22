# deep-learning-challenge

# Alphabet Soup Charity Success Prediction

## Overview
This repository contains a deep learning project aimed at predicting the success of funding applications for the Alphabet Soup charity organization. The project leverages a neural network model built with TensorFlow and Keras to identify patterns in historical data that correlate with successful applications.

## Project Structure
- `model/`
  - `trained_model.h5`: A saved model in HDF5 format.
- `data/`
  - `charity_data.csv`: The dataset used for training and evaluation.
- `scripts/`
  - `preprocessing.py`: Data preprocessing script.
  - `train.py`: Script to train the neural network.
  - `evaluate.py`: Script to evaluate the model performance.
- `notebooks/`
  - `model_training.ipynb`: Jupyter Notebook detailing the model training and evaluation process.
- `requirements.txt`: List of dependencies for the project.

## Results
The 3 neural network model consisted of two to four hidden layers and was trained on a dataset containing various application features. The target feature was the success of the application, and several variables were considered in the prediction process. The model achieved approximately 74% accuracy on both training and test sets.

### Data Preprocessing
- The target variable was 'IS_SUCCESSFUL'.
- Feature variables included 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', and several others.
- Non-informative variables such as 'EIN' and 'NAME' were removed.

### Model Performance
- The neural network model had 80 neurons in the first hidden layer and 30 neurons in the second.
- The model used 'relu' activation functions in the hidden layers and 'sigmoid' for the output layer.
- The final model achieved an accuracy of ~74.66% on the test data, with a loss of 0.531.

## Installation
To set up the project environment, run the following command to install the required packages:
pip install - tensorflow


## Usage
To train the model, run:
python scripts/train.py
To evaluate the model, run:
python scripts/evaluate.py

## Contributions
Contributions to this project are welcome. 

## License
Distributed by IRS. Tax Exempt Organization Search Bulk Data Downloads. https://www.irs.gov/

## Contact
Nick Nath

## Acknowledgements
- Alphabet Soup Dataset
- Data analytics bootcamp for providing the dataset
  

