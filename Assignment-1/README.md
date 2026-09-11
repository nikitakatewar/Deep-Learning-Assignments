# Deep Learning Assignment 1

## Problem Statement

Install and configure TensorFlow/Keras in Google Colab. Perform data preprocessing, normalization, train-test split, and visualization on the Fashion MNIST dataset.

## Dataset

**Fashion MNIST Dataset**

Fashion MNIST is an image classification dataset consisting of 28 × 28 grayscale images belonging to 10 different classes.

## Tools and Technologies

- Python
- Google Colab
- TensorFlow
- Keras
- Matplotlib

## Algorithm

1. Import TensorFlow and Matplotlib libraries.
2. Load the Fashion MNIST dataset using TensorFlow/Keras.
3. Split the dataset into training and testing datasets.
4. Normalize the image pixel values.
5. Display the shape of training images, testing images, and labels.
6. Create a Sequential neural network model.
7. Train the model using the training dataset for 3 epochs.
8. Evaluate the model using the testing dataset.
9. Display the test accuracy.
10. Save the trained model as `fashion_mnist_model.keras`.

## Model Architecture

The Sequential neural network consists of:

- Flatten layer with input shape `(28, 28)`
- Dense layer with 128 neurons and ReLU activation
- Dense output layer with 10 neurons and Softmax activation

## Implementation

The Fashion MNIST dataset was loaded and the image pixel values were normalized by dividing them by 255.0.

The dataset was visualized using Matplotlib. A Sequential neural network was then created, compiled using the Adam optimizer and Sparse Categorical Crossentropy loss function, and trained for 3 epochs.

## Result

The model was successfully trained and evaluated on the Fashion MNIST test dataset.

**Test Accuracy: 85.13%**

The trained model was saved as:

`fashion_mnist_model.keras`

## Conclusion

The Fashion MNIST dataset was successfully preprocessed, visualized, and classified using a Sequential neural network in TensorFlow/Keras. The model achieved a test accuracy of approximately 85.13%.
