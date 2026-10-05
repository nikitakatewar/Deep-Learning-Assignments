# Assignment 8 

## Problem Statement

Implement a pre-trained BERT model for sentiment analysis or text classification on a sample dataset.

## Objective

To implement a pre-trained BERT (`bert-base-uncased`) model for binary sentiment classification and predict whether a given text is positive or negative.

## Description

BERT (Bidirectional Encoder Representations from Transformers) is a pre-trained Natural Language Processing (NLP) model developed by Google. It is based on the Transformer architecture and understands the context of words by considering both the left and right sides of a word.

In this practical, the `bert-base-uncased` model is used for binary sentiment classification:

- `0` → Negative
- `1` → Positive

The BERT tokenizer converts text into tokens and numerical IDs that can be processed by the BERT model.

## Technologies Used

- Python
- Google Colab
- PyTorch
- Hugging Face Transformers
- Hugging Face Datasets
- NumPy
- Pandas
- Scikit-learn

## Model Used

**Pre-trained Model:** `bert-base-uncased`

**Classification Model:** `BertForSequenceClassification`

The model is configured for two output classes: Positive and Negative.

## Methodology

1. Create a sample sentiment dataset containing text and corresponding labels.
2. Split the dataset into training and testing sets using an 80:20 split.
3. Load the pre-trained BERT tokenizer.
4. Tokenize the text data.
5. Create datasets containing tokenized inputs and labels.
6. Load `bert-base-uncased` for sequence classification.
7. Train the model for 3 epochs.
8. Evaluate the model on the test dataset.
9. Generate predictions.
10. Calculate accuracy, precision, recall, and F1-score.
11. Generate a confusion matrix.
12. Test the model on a new sentence.

## Training Parameters

| Parameter               | Details                    |
| ----------------------- | -------------------------- |
| **Pre-trained Model**   | bert-base-uncased          |
| **Number of Classes**   | 2 (Negative, Positive)     |
| **Number of Epochs**    | 3                          |
| **Training Batch Size** | 4                          |
| **Testing Batch Size**  | 4                          |
| **Train-Test Split**    | 80% Training / 20% Testing |


## Results

The model achieved:

- **Test Accuracy:** - 50%
- **Test Loss:** - 0.6721

### Classification Report

| Class                | Precision | Recall | F1-Score | Support |
| -------------------- | --------: | -----: | -------: | ------: |
| **Negative**         |      0.50 |   1.00 |     0.67 |       2 |
| **Positive**         |      0.00 |   0.00 |     0.00 |       2 |
| **Accuracy**         |         — |      — | **0.50** |   **4** |
| **Macro Average**    |      0.25 |   0.50 |     0.33 |       4 |
| **Weighted Average** |      0.25 |   0.50 |     0.33 |       4 |


### Confusion Matrix

| **Actual / Predicted** | **Negative (0)** | **Positive (1)** |
| ---------------------- | ---------------: | ---------------: |
| **Negative (0)**       |                2 |                0 |
| **Positive (1)**       |                2 |                0 |
