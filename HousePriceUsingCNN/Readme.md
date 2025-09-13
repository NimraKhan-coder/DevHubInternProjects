Real Estate Price Prediction (Tabular + Image Data)
Overview

This project implements a deep learning model that predicts house prices using a combination of tabular data (numerical and categorical features) and image data (house photographs). The approach integrates a Convolutional Neural Network (CNN) for image feature extraction and a Multi-Layer Perceptron (MLP) for tabular data, merged into a hybrid architecture.
Dataset Description

socal2.csv contains structured data with the following columns:

street → Street name

city → City name

city_num → Encoded city identifier

bed → Number of bedrooms

bath → Number of bathrooms

sqft → Square footage of the property

price → Target variable (house price)

image_id → Identifier linking to the corresponding house image

socal_pics/ contains .jpg images of houses, named according to image_id

Preprocessing Workflow

Load the dataset with pandas.

Rename selected columns for clarity (citi → city, n_citi → city_num).

Encode categorical features (street, city) using LabelEncoder.

Standardize numerical features with StandardScaler.

Load, resize, and normalize images with OpenCV.

Model Architecture

Image branch (CNN):

Convolutional and pooling layers for feature extraction

Flatten + Dense layers for representation learning

Tabular branch (MLP):

Dense layers for numerical and categorical features

Fusion:

Concatenate CNN and MLP outputs

Final Dense layer for regression (price prediction)

Training setup:

Loss function: Mean Squared Error (MSE)

Optimizer: Adam with learning rate scheduling

Metric: Mean Absolute Error (MAE)

Evaluation

Loss curves are plotted to compare training and validation performance.

Metrics monitored:

Training loss (loss)

Validation loss (val_loss)

Mean Absolute Error (mae)

