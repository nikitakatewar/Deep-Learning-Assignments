# Deep Learning Assignment 5

## Problem Statement

Implement and compare RNN, LSTM, and GRU models for sequence classification, and analyze their performance using appropriate evaluation metrics.

## Dataset

**IMDB Movie Review Dataset**

The IMDB dataset is used for binary sentiment classification of movie reviews.

## Tools and Technologies

- Python
- Google Colab
- TensorFlow/Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Models Used

- Simple RNN
- LSTM
- GRU

## Algorithm

1. Load the IMDB movie review dataset.
2. Preprocess and prepare the text sequences.
3. Create RNN, LSTM, and GRU models.
4. Train each model for 3 epochs.
5. Predict the sentiment of test reviews.
6. Evaluate the models using accuracy, precision, recall, and F1-score.
7. Generate confusion matrices.
8. Compare the performance of all three models.

## Results

| Model | Accuracy | Precision | Recall | F1 Score |

| RNN | 84.54% | 83.24% | 86.51% | 84.84% |
| LSTM | 85.67% | 81.60% | 92.11% | 86.54% |
| GRU | 84.22% | 88.53% | 78.63% | 83.29% |

The LSTM model achieved the highest accuracy of **85.67%** in this experiment.

## Conclusion

RNN, LSTM, and GRU models were successfully implemented for IMDB sentiment classification. Their performance was evaluated using accuracy, precision, recall, F1-score, and confusion matrices.
