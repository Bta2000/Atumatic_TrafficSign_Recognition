# Automatic Traffic Sign Recognition using CNN

A deep learning project for automatic traffic sign recognition using a Convolutional Neural Network (CNN).

This project was developed as my **Bachelor's final project in Computer Engineering** and focuses on classifying traffic signs using image preprocessing, data augmentation, and a CNN-based classification model.

## Overview

Traffic sign recognition is an important application of computer vision and intelligent transportation systems.

The goal of this project is to build a CNN-based model capable of recognizing different categories of traffic signs from images.

The project uses the **German Traffic Sign Recognition Benchmark (GTSRB)** dataset and performs image preprocessing, data augmentation, model training, validation, and prediction.

## Dataset

The project uses the **German Traffic Sign Recognition Benchmark (GTSRB)** dataset.

The dataset contains traffic sign images belonging to **43 different classes**.

The images are processed before being provided to the neural network. The preprocessing pipeline includes:

* Converting images to grayscale
* Histogram equalization
* Normalization
* Resizing images to `32 × 32`
* Splitting the available data into training and validation sets

## Preprocessing

The following preprocessing steps are applied to the input images:

1. Images are loaded from the dataset.
2. Images are converted to grayscale.
3. Histogram equalization is applied to improve image contrast.
4. Images are resized to `32 × 32` pixels.
5. Pixel values are normalized.
6. The processed data is divided into training and validation sets.

Data augmentation is also used during training to increase the variety of training samples and improve the model's ability to generalize.

## CNN Model

A Convolutional Neural Network is used as the main classification model.

The architecture includes:

* Convolutional layers
* Max pooling layers
* Dropout layers
* A fully connected classification layer
* A Softmax output layer for the 43 traffic sign classes

The model is trained using:

* **Optimizer:** Adam
* **Loss function:** Categorical Cross-Entropy
* **Epochs:** 30
* **Batch size:** 500

## Results

The model achieved a validation accuracy of approximately **97.81%** during training.

The notebook also includes prediction examples for test images. For each prediction, the model provides the most probable traffic sign classes along with their corresponding probabilities.

## Technologies

* Python
* TensorFlow / Keras
* NumPy
* Pandas
* OpenCV
* Matplotlib
* Scikit-learn
* Jupyter Notebook

## Project Structure

```text
Atumatic_TrafficSign_Recognition/
│
├── Automatic Traffic Sign Recognition_CNN.ipynb
├── Automatic Traffic Sign Recognition CNN.pdf
├── ECAI50035.2020.9223186.pdf
└── README.md
```

### Files

**`Automatic Traffic Sign Recognition_CNN.ipynb`**
Contains the complete implementation of the project, including data loading, preprocessing, model definition, training, evaluation, and prediction.

**`Automatic Traffic Sign Recognition CNN.pdf`**
The Persian project report prepared for the Bachelor's final project.

**`ECAI50035.2020.9223186.pdf`**
The research paper used as a reference for the project.

## How to Run

1. Clone the repository.

2. Download the GTSRB dataset and extract it on your local machine.

3. Open the Jupyter Notebook:

```text
Automatic Traffic Sign Recognition_CNN.ipynb
```

4. Update the dataset paths in the notebook according to the location of the dataset on your own system.

The original notebook uses local paths similar to:

```python
dataset_folder = 'E:/Downloads/Compressed/final dataset/GTSRB_Final_Training_Images'
test_folder = 'E:/Downloads/Compressed/final dataset/GTSRB_Final_Test_Images'
```

These paths are specific to the original development environment and should be changed to the corresponding paths on the user's machine.

5. Run the notebook cells sequentially.

## Reference

The project was developed with reference to the following research paper:

**ECAI50035.2020.9223186**

The original paper is included in this repository for reference.

## Project Report

The complete Bachelor's project report is available in Persian:

**Automatic Traffic Sign Recognition CNN.pdf**

## Academic Context

This project was completed as my **Bachelor's final project in Computer Engineering**.

## Author

**Bita Shahani**

GitHub: [Bta2000](https://github.com/Bta2000)
