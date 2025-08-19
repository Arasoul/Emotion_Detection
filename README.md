# Emotion_Detection

## Project Overview
This project implements an emotion detection system using deep learning (TensorFlow/Keras) to classify facial expressions into emotions. It uses the FER2013 dataset for training and validation, and applies an ensemble of convolutional neural networks (CNNs) for improved accuracy.

## Features
- Downloads and preprocesses the FER2013 dataset (grayscale, 48x48 images)
- Data augmentation for robust training
- CNN model with regularization, dropout, and batch normalization
- Ensemble learning: trains three models and combines their predictions
- Visualizes training/validation loss and accuracy
- Predicts emotions from new images and displays results using OpenCV

## Usage
1. Download the FER2013 dataset from Kaggle (`vipulpisal/fer2013-updated`).
2. Run the notebook `Emotion-Detecion.ipynb` to train models and make predictions.
3. Place new images in the specified folder to test emotion detection.

## Requirements
- Python 3.x
- TensorFlow
- Keras
- scikit-learn
- pandas
- numpy
- matplotlib
- PIL
- OpenCV

## How it Works
1. The notebook loads and preprocesses the dataset.
2. Three CNN models are trained with early stopping and data augmentation.
3. Ensemble predictions are made for validation and new images.
4. Results are visualized and printed for each test image.

## Example Output
```
PhotoName: test1.jpg, Predicted Emotion: happy
PhotoName: test2.jpg, Predicted Emotion: sad
```

## License
See repository for license details.
