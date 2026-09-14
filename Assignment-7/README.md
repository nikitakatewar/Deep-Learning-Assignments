# Deep Learning Assignment 7

## Problem Statement

Implement transfer learning using pre-trained VGG16 and ResNet50 models for image classification, and compare their performance.

## Dataset

**CIFAR-10 Dataset**

CIFAR-10 is an image classification dataset containing 10 different classes.

The 10 classes are:

- Airplane
- Automobile
- Bird
- Cat
- Deer
- Dog
- Frog
- Horse
- Ship
- Truck

The original CIFAR-10 dataset contains 50,000 training images and 10,000 testing images.

For this experiment, a smaller balanced dataset was created by selecting:

- 100 images per class for training
- 20 images per class for testing

Therefore:

- Training images: 1,000
- Testing images: 200

## What is Transfer Learning?

Transfer learning is a deep learning technique in which a model that has already been trained on a large dataset is reused for a new but related task.

In this experiment, pre-trained VGG16 and ResNet50 models with ImageNet weights are used for feature extraction and CIFAR-10 image classification.

## Models Used

Two pre-trained models were implemented:

1. VGG16
2. ResNet50

## Tools and Technologies

- Python
- Google Colab
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib

## Algorithm

1. Import the required Python libraries.
2. Load the CIFAR-10 dataset.
3. Define the names of the 10 classes.
4. Create a smaller balanced training and testing dataset.
5. Visualize sample images from different classes.
6. Flatten the class labels.
7. Resize the CIFAR-10 images from 32 × 32 to 96 × 96 pixels.
8. Create TensorFlow training and testing datasets.
9. Load the pre-trained VGG16 model with ImageNet weights.
10. Freeze the pre-trained VGG16 layers.
11. Add Global Average Pooling, Dense, Dropout, and Softmax layers.
12. Compile and train the VGG16 model.
13. Evaluate the VGG16 model and record its accuracy.
14. Load the pre-trained ResNet50 model with ImageNet weights.
15. Freeze the pre-trained ResNet50 layers.
16. Add the required classification layers.
17. Compile and train the ResNet50 model.
18. Evaluate the ResNet50 model and record its accuracy.
19. Compare the performance of VGG16 and ResNet50.
20. Display the comparison using a graph.

## VGG16 Model Architecture

The VGG16 transfer learning model consists of:

- Pre-trained VGG16 base model
- ImageNet pre-trained weights
- Frozen VGG16 layers
- Global Average Pooling layer
- Dense layer with 128 neurons and ReLU activation
- Dropout layer with dropout rate 0.5
- Dense output layer with 10 neurons
- Softmax activation

## ResNet50 Model Architecture

The ResNet50 transfer learning model consists of:

- Pre-trained ResNet50 base model
- ImageNet pre-trained weights
- Frozen ResNet50 layers
- Global Average Pooling layer
- Classification layers
- Softmax output layer for 10 CIFAR-10 classes

## Image Preprocessing

The original CIFAR-10 images have a size of:

`32 × 32 × 3`

The images were resized to:

`96 × 96 × 3`

## Model Training

The models were trained using:

- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Epochs: 3
- Batch Size: 32
- Pre-trained layers: Frozen


### Performance Comparison

- **VGG16 Accuracy:** 52.00%
- **ResNet50 Accuracy:** 62.00%
- **Better Performing Model:** ResNet50

ResNet50 achieved higher test accuracy than VGG16 in this experiment.

## Conclusion

Transfer learning using pre-trained VGG16 and ResNet50 models was successfully implemented for CIFAR-10 image classification.

The CIFAR-10 images were resized from 32 × 32 to 96 × 96 pixels. The pre-trained layers of both models were frozen and used for feature extraction, while new classification layers were added for the 10 CIFAR-10 classes.

The experimental results show that ResNet50 achieved better performance than VGG16, with an accuracy of 62.00% compared to 52.00% for VGG16.

## Files

- `DL_Assi7.ipynb` – Google Colab notebook containing the implementation and outputs.
- `DL_Assi7.docx` – Practical implementation sheet.
- `README.md` – Description and details of Assignment 7.
