# Fruit Classification

## About the Project

This project is an image classification system designed to recognize five different types of fruits using a Convolutional Neural Network (CNN).

The model classifies fruit images into the following categories:

- Apple
- Banana
- Grape
- Mango
- Strawberry

This project was developed using Python and TensorFlow/Keras as part of a machine learning project.

## Objective

The main objective of this project is to build a deep learning model that can classify fruit images into their corresponding categories based on visual features.

The project also demonstrates the implementation of image preprocessing, data augmentation, CNN model development, model training, and model evaluation.

## Dataset

The dataset consists of images belonging to five fruit classes:

| Class | Description |
|---|---|
| Apple | Images of apples |
| Banana | Images of bananas |
| Grape | Images of grapes |
| Mango | Images of mangoes |
| Strawberry | Images of strawberries |

The dataset is divided into training, validation, and testing sets.

- Training images: 9,715
- Validation images: 200
- Testing images: 100
- Image size: 128 × 128 pixels

## Method

The project follows several steps:

1. Load and prepare the image dataset.
2. Resize images to 128 × 128 pixels.
3. Apply image preprocessing.
4. Apply data augmentation to the training images.
5. Build a Convolutional Neural Network (CNN).
6. Train the model using the training dataset.
7. Monitor validation performance during training.
8. Use Early Stopping to help prevent unnecessary training.
9. Evaluate the trained model using the test dataset.

### Data Augmentation

Data augmentation is applied to the training images to increase variation in the training data.

The augmentation includes:

- Rotation
- Zoom
- Width and height shifting
- Horizontal flipping

## Model Architecture

The classification model uses a Convolutional Neural Network (CNN).

The architecture includes:

- Convolutional layers
- MaxPooling layers
- Dense (fully connected) layers
- Dropout layer
- Softmax output layer for five fruit classes

The model is compiled using the Adam optimizer with a learning rate of `0.0005`.

The training process is configured for a maximum of 100 epochs and uses Early Stopping.

## Results

The trained model was evaluated using the test dataset.

**Test Accuracy: 82%**

**Test Loss: 0.6132**

### Training Accuracy

![Training Accuracy](assets/accuracy.png)

### Training Loss

![Training Loss](assets/loss.png)

### Confusion Matrix

![Confusion Matrix](assets/confusion-matrix.png)

## Tools & Technologies

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Jupyter Notebook / Google Colab
- Convolutional Neural Network (CNN)

## Project Structure

```text
fruit-classification/
│
├── fruit-classification.ipynb
└── README.md
