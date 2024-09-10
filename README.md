# Face Recognition with GoogleNet

This project implements a facial recognition system using a deep learning approach with GoogleNet. It includes training the model with an augmented image dataset and testing it via webcam input. The system captures images, resizes them, classifies them using a pre-trained network, and displays the results.

## Key Steps:

### 1. Training the Model:
- We utilized the **GoogleNet architecture** to train a model for facial recognition. The dataset is split into training and validation sets, with labels sourced from folder names.
- Layers 142 and 144 of GoogleNet are replaced with a **fully connected layer** and a **classification layer**, customized for facial recognition based on the number of facial classes.
- **Image augmentation** techniques such as random reflection, translation, and scaling are applied to increase model robustness and improve generalization.
- The model is trained using **Stochastic Gradient Descent with Momentum (SGDM)**, and the training progress is visualized using MATLAB's tools.

### 2. Testing the Model:
- The trained model is tested using **real-time images captured from a webcam**.
- Each captured image is resized to match GoogleNet’s input size (224x224) and classified using the trained model.
- The image is then displayed alongside the predicted label and confidence score.

## Features:
- **Dataset Augmentation**: Enhances model generalization by introducing variations in the training data.
- **Custom Layer Integration**: GoogleNet’s feature extraction layers are fine-tuned for facial recognition.
- **Real-Time Testing**: Captures images from a webcam and performs classification on-the-fly, displaying the result.

## Technologies Used:
- **MATLAB**: For training, augmenting images, and performing real-time classification.
- **GoogleNet**: A pre-trained Convolutional Neural Network (CNN) modified for facial feature extraction and classification.

This project provides a robust framework for facial recognition, which can be further adapted for other image classification tasks.

Some of the images were collected from Google Images. 
