# Deep Learning Assignment 6


## Problem Statement

Design and implement a Convolutional Neural Network (CNN) for image classification using the Tomato or Soybean disease dataset.

## Dataset

**Tomato Disease Dataset**

The Tomato Disease Dataset contains images of tomato leaves belonging to different disease classes.

The CNN takes a tomato leaf image as input and predicts its disease class.

## Tools and Technologies

- Python
- Google Colab
- TensorFlow
- Keras
- NumPy
- Matplotlib

## Algorithm

1. Load the Tomato Disease Dataset containing training and validation images.
2. Identify the different disease classes present in the dataset.
3. Resize all input images to a fixed size of 128 × 128 pixels.
4. Load the training and validation datasets using TensorFlow/Keras.
5. Create a Convolutional Neural Network (CNN) model.
6. Add a convolution layer with 32 filters and ReLU activation.
7. Add a 2 × 2 Max Pooling layer.
8. Add a convolution layer with 128 filters and ReLU activation.
9. Add a Dense layer containing 128 neurons with ReLU activation.
10. Add a Dropout layer to reduce overfitting.
11. Train the CNN using the training dataset.
12. Validate the model using the validation dataset.
13. Calculate validation accuracy and loss.
14. Plot training and validation accuracy and loss graphs.
15. Generate a classification report containing precision, recall, and F1-score.

## CNN Architecture

The CNN model consists of:

- Input images resized to 128 × 128 pixels
- Convolutional layer with 32 filters
- ReLU activation
- MaxPooling2D with pool size 2 × 2
- Convolutional layer with 128 filters
- ReLU activation
- Dense layer with 128 neurons
- ReLU activation
- Dropout layer
- Output layer with Softmax activation

## Activation Functions

### ReLU

ReLU (Rectified Linear Unit) is used in the convolutional and dense layers.

Formula:

`ReLU(x) = max(0, x)`

It converts negative values to zero and keeps positive values.

### Softmax

The final output layer uses Softmax activation to provide a probability for each disease class.

The class with the highest probability is considered the predicted class.

## Data Preprocessing

The input images are:

- Resized to 128 × 128 pixels.
- Normalized from the range 0–255 to 0–1.

## Evaluation Measures

The CNN performance is evaluated using:

- **Accuracy** – Percentage of correctly classified images.
- **Loss** – Measures the error between actual and predicted classes.
- **Confusion Matrix** – Shows correct and incorrect predictions for each disease class.
- **Precision** – Measures how many predicted positive samples are actually correct.
- **Recall** – Measures how many actual positive samples are correctly identified.
- **F1-score** – Harmonic mean of precision and recall.

## Result

The Convolutional Neural Network was successfully implemented using TensorFlow/Keras for tomato leaf disease classification.

The model performance was evaluated using accuracy, loss, confusion matrix, precision, recall, and F1-score.

Training and validation accuracy and loss graphs were also generated.

## Conclusion

The Convolutional Neural Network (CNN) was successfully designed and implemented using TensorFlow/Keras for tomato leaf disease classification. The CNN automatically extracts important features from tomato leaf images using convolution and pooling layers and classifies the leaves into different disease classes.

The model performance was evaluated using accuracy, loss, confusion matrix, precision, recall, and F1-score. The experiment demonstrates that CNN can be effectively used for tomato disease image classification.
