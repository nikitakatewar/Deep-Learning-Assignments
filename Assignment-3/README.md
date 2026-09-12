# Deep Learning Assignment 3

## Problem Statement

Implement forward propagation and backpropagation using TensorFlow/Keras. Analyze the effect of different learning rates and the number of epochs on model performance.

## Dataset

**Iris Dataset**

The Iris dataset is used for classification.

- Number of samples: 150
- Number of input features: 4
- Number of classes: 3

The classes are:
- Setosa
- Versicolor
- Virginica

## Tools and Technologies

- Python
- Google Colab
- NumPy
- Pandas
- Matplotlib
- TensorFlow
- Keras

## Algorithm

1. Import the required libraries such as NumPy, Pandas, Matplotlib and TensorFlow/Keras.
2. Load the Iris dataset.
3. Separate the input features and target labels.
4. Split the dataset into training and testing sets.
5. Create a Sequential neural network model.
6. Add Dense layers with ReLU activation.
7. Add an output layer with Softmax activation for classification.
8. Compile the model using the Adam optimizer and Sparse Categorical Crossentropy loss.
9. Perform forward propagation to obtain the predicted output.
10. Use backpropagation to update the weights and biases during training.
11. Train the model using different learning rates.
12. Evaluate the model using test accuracy.
13. Train the model using different numbers of epochs.
14. Compare the accuracy obtained for different learning rates and epochs.
15. Plot the required graphs.

## Model Architecture

The neural network consists of:

- Input layer with 4 features
- Dense layer with 16 neurons and ReLU activation
- Dense layer with 8 neurons and ReLU activation
- Output layer with 3 neurons and Softmax activation

### Optimizer

Adam Optimizer

### Loss Function

Sparse Categorical Crossentropy

## Learning Rate Analysis

The model was trained using different learning rates and the test accuracy was compared.

| Learning Rate | Test Accuracy |
|---:|---:|
| 0.1 | 100% |
| 0.01 | 100% |
| 0.001 | 90% |

The results show that the learning rate affects the performance of the neural network.

## Epoch Analysis

The model was trained using different numbers of epochs.

| Number of Epochs | Test Accuracy |
|---:|---:|
| 10 | 53.33% |
| 50 | 73.33% |
| 100 | 90.00% |

The results show that increasing the number of epochs improved the model performance for this experiment.

## Forward Propagation

Forward propagation is the process of passing the input data through the neural network layers to calculate the predicted output.

## Backpropagation

Backpropagation is the process of calculating the error and updating the weights and biases of the neural network during training.

## Result

Forward propagation and backpropagation were successfully implemented using TensorFlow/Keras on the Iris dataset.

The effect of different learning rates and numbers of epochs was analyzed using test accuracy.


## Conclusion

Forward propagation and backpropagation were successfully implemented using TensorFlow/Keras. The effect of different learning rates and numbers of epochs on model performance was analyzed. The experiment demonstrates that hyperparameters such as learning rate and number of epochs can affect the performance of a neural network.
