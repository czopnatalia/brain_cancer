## Collaborators:
@czopnatalia, @AndKac600224, @victoriabelz, @Karo2604, @JakubHus

# Brain Tumor Image Classification with CNN (Convolutional Neural Networks)

This project implements an **image classification system using Convolutional Neural Networks (CNN)** built with **TensorFlow and Keras**. The goal is to classify MRI brain images into two categories: **tumor present ("yes")** or **no tumor ("no")**.

The repository demonstrates a **complete deep learning pipeline**, including data loading, model training, validation, and performance evaluation.

---

# Project Overview

The model is trained on MRI brain images and learns to identify patterns associated with brain tumors. The pipeline includes:

- loading and preprocessing image datasets
- training a CNN model
- validating model performance
- evaluating the trained model on unseen test data
- generating performance metrics and a confusion matrix

---

## Project Structure
Brain_Cancer_TF_AI/   
├── train_model.py # Script for training the CNN model  
├── eval_model.py # Script for evaluating the trained model  
├── dataset/ # Dataset directory (not included in the repository)  
│ ├── training/   
│ ├── validation/   
│ └── testing/   
└── README.md   

**Note:** The dataset is not included in the repository due to its size.

Dataset download:  
https://drive.google.com/drive/folders/19FRUtOCDf6yd7PUP5lGurRDn0h1uYFAO

---

# Dataset Format

The dataset must follow this structure:

dataset/  
├── training/  
│ ├── yes/  
│ ├── no/  
├── validation/    
│ ├── yes/  
│ ├── no/  
└── testing/  
├── yes/  
├── no/  

Each folder should contain images corresponding to a single class.

---

# Model Architecture

The implemented CNN architecture includes:

- Convolutional layers with **ReLU activation**
- **MaxPooling layers** for spatial downsampling
- **Flatten layer** to convert feature maps into vectors
- **Dense layers** for classification
- **Dropout layers** to reduce overfitting
- **Softmax output layer** for class prediction

---

## Train the model

To train the model, run:

```bash
python train_model.py

This script will:
* Load training and validation datasets.
* Build and compile the CNN model.
* Train the model using EarlyStopping.
* Save the best performing model as: `best_model_postx.keras`

## Evaluate the model

After training, run the evaluation script:

```bash
python eval_model.py

This script will:
* Load the trained model 
* Evaluate the model on training, validation, and testing datasets.
* Display a confusion matrix and a detailed classification report.


## Metrics tracked during training:
* Accuracy
* Precision
* Recall

## Technologies Used

Python, TensorFlow / Keras, NumPy, Matplotlib, Scikit-learn


## Example outputs
<img width="564" height="407" alt="image" src="https://github.com/user-attachments/assets/3d04d44f-58f3-4612-b251-458143c29e05" />
<img width="777" height="622" alt="image" src="https://github.com/user-attachments/assets/5cb23451-47ad-424d-aa36-805950cb74c3" />

## Summary   
Authors: Natalia Czop and collaborators mentioned before
Project Type: Deep Learning / Image Classification / AI / Convolutional Neural Network

