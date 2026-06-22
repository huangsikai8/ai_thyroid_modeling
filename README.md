# AI Analysis of Thyroid Ultrasound Images for Early Cancer Detection and Risk Management

An AI-powered system that analyzes thyroid ultrasound images and automatically generates ACR TI-RADS scores to assist clinicians in thyroid cancer risk assessment.

## Motivation

Manual interpretation of thyroid ultrasound images can be time-consuming and subject to inter-observer variability. This project explores the use of deep learning to automate the classification of thyroid nodule characteristics and provide explainable risk assessments.

## Features

- Automated analysis of thyroid ultrasound images
- Prediction of key ACR TI-RADS characteristics:
  - Echogenicity
  - Margin
  - Macrocalcification
  - Punctate Echogenic Foci
- Automatic TI-RADS score calculation
- Python Tkinter graphical user interface
- Explainable predictions aligned with clinical guidelines

## Dataset

- 79 thyroid ultrasound images
- 15 patients
- Data augmentation applied to improve model robustness
- Train / Validation / Test split: 70% / 15% / 15%

## Model

A lightweight VGG-inspired convolutional neural network architecture was used to classify individual TI-RADS characteristics.

Training configuration:

- Adam optimizer
- Learning rate: 5e-5
- Batch size: 32
- 50 epochs
- L2 regularization

## Results

| Characteristic | F1 Score |
|---------------|----------|
| Echogenicity | 0.90 |
| Margin | 0.87 |
| Macrocalcification | 0.83 |
| Punctate Echogenic Foci | 0.83 |

The system achieved comparable performance to larger published models while requiring significantly less computational resources.

## Screenshots

Add screenshots of:
- GUI interface
- Example prediction output
- Model architecture (optional)

## Tech Stack

- Python
- TensorFlow / Keras
- OpenCV
- NumPy
- Tkinter

## Future Improvements

- Larger dataset
- Additional TI-RADS characteristics
- Web-based deployment
- Clinical validation on external datasets

## Authors

- Sikai Huang
- Buyan Hu
- Cheryl Koh

## Disclaimer

This project was developed for research and educational purposes and is not intended for clinical use.