# Malaria Cell Classification Using Convolutional Neural Networks (CNN)

## Overview
This project uses a Convolutional Neural Network (CNN) to classify cell images as either **Parasitized** (infected with malaria) or **Uninfected**. The model processes image data, extracts meaningful features, and applies deep learning to achieve high accuracy in classification.

---

## Features
- **Data Preprocessing**: Images are resized, normalized, and labeled to prepare them for training.
- **CNN Architecture**: Multi-layered network with convolutional, pooling, normalization, and dropout layers.
- **Training and Evaluation**: Assesses performance with accuracy and loss metrics.
- **Visualization**: Graphs of training performance (accuracy and loss).
- **Model Saving**: Trained model saved for deployment or further use.

---

## Workflow

### 1. Data Preparation
- Images from the `Parasitized` and `Uninfected` directories are resized to 64x64 pixels and converted to NumPy arrays. 
- Labels:
  - `0`: Parasitized
  - `1`: Uninfected

### 2. CNN Architecture
The CNN includes:
- **Input Layer**: Processes 64x64x3 RGB images.
- **Convolutional Layers**: Extract features from images.
- **Pooling Layers**: Reduce spatial dimensions.
- **Batch Normalization and Dropout**: Improves training speed and reduces overfitting.
- **Dense Layers**: Fully connected layers for classification.
- **Output Layer**: Sigmoid activation for binary classification.

### 3. Training
- **Data split**: 80% training, 20% testing.
- **Optimizer**: Adam
- **Loss Function**: Categorical Crossentropy
- **Metrics**: Accuracy

### 4. Evaluation
- Computes test accuracy.
- Visualizes training and validation performance (accuracy and loss).

### 5. Model Saving
- The trained model is saved as `malaria_cnn.h5`.

---

## Prerequisites

### Required Libraries
Ensure the following Python libraries are installed:
- NumPy
- Matplotlib
- OpenCV (cv2)
- TensorFlow/Keras
- PIL (Pillow)


<h2>Dataset:</h2> 
https://drive.google.com/file/d/1xD4r84RYExkFflsZ2VLytJs658kECj_L/view?usp=sharing
<br>
<br>
***Malarial cell claffication using a CNN from stratch.***

Malaria is a mosquito-borne infectious disease that affects humans and other animals. Malaria causes symptoms that typically include fever, tiredness, vomiting, and headaches. In severe cases, it can cause yellow skin, seizures, coma, or death.
<br>
Malaria parasites can be identified by examining under the microscope a drop of the patient's blood, spread out as a “blood smear” on a microscope slide. Prior to examination, the specimen is stained (most often with the Giemsa stain) to give the parasites a distinctive appearance.
<br>
<h2>Uninfected and Parasitized cells:</h2>
<img align="center" width="400" height="250" src="https://github.com/devanshpratapsingh/Malarial-Cell-Classification/blob/main/images/img1.jpg">

## Installation and Quick Start
To use the repo, please follow the guidelines below:

- Clone the Repository: 

        $ git clone https://github.com/devanshpratapsingh/Malarial-Cell-Classification.git
        
- Enter the directory: 

        $ cd Malarial-Cell-Classification
        
- Install the requirements:

        $ pip install -r requirements.txt

- For running:

        open Malarial_Cell_Classification.py
	


*With this, I hope you liked the project, if you did please make sure to leave a star. Thanks!*

