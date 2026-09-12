# Deep Learning Assignment 2

## Problem Statement

Design and implement a Multilayer Perceptron (MLP) for classification of the Iris or Wine dataset, and evaluate its performance using accuracy and a confusion matrix.

## Dataset

**Iris Dataset**

The Iris dataset from Scikit-learn is used for classification.

- Number of samples: 150
- Number of features: 4
- Number of classes: 3

The classes are:
- Setosa
- Versicolor
- Virginica

## Tools and Technologies

- Python
- Google Colab
- NumPy
- Matplotlib
- Scikit-learn
- MLPClassifier

## Algorithm

1. Import the required Python libraries.
2. Load the Iris dataset from Scikit-learn.
3. Separate the dataset into input features (X) and target labels (y).
4. Normalize the input features using StandardScaler.
5. Split the dataset into training and testing sets.
6. Create MLP models with different hidden layer configurations.
7. Train the MLP models using the training dataset.
8. Predict the class labels for the testing dataset.
9. Calculate Accuracy, Precision, Recall, and F1-Score.
10. Generate the Confusion Matrix.
11. Visualize the Confusion Matrix.
12. Plot the training Loss Curve.
13. Display the evaluation results and graphs.

## MLP Models

### MLP Model 1

- Hidden layers: `(100, 100)`
- Maximum iterations: `2000`
- Learning rate: `0.001`

### MLP Model 2

- Hidden layer: `(50,)`
- Maximum iterations: `2000`
- Learning rate: `0.001`

## Result

Both MLP models achieved the following performance on the test dataset:

| Metric     | MLP Model 1 | MLP Model 2 |

| Accuracy   | 1.00        | 1.00 |
| Precision  | 1.00        | 1.00 |
| Recall     | 1.00        | 1.00 |
| F1-Score   | 1.00        | 1.00 |

The confusion matrix and training loss curve were also generated successfully.


## Conclusion

The Multilayer Perceptron models were successfully implemented on the Iris dataset using Scikit-learn. The dataset was standardized using StandardScaler and the models were evaluated using accuracy, precision, recall, F1-score, and confusion matrix. Both models achieved an accuracy of 1.00 on the test dataset.
