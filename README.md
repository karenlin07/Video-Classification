# Video Classification with CNN and LSTM
This project implements a video classification model using a combination of Convolutional Neural Networks (CNN) and Long Short-Term Memory (LSTM) networks. The model is designed to take video frames, extract spatial features using a CNN, and process temporal dependencies between frames using an LSTM. The final output is a classification of the video into one of 10 classes.

**Project Structure**  
VideoModel.py: Contains the implementation of the VideoModel class, which is used for video classification.  
train.py: The script to train the model.  
evaluation.py: Code to evaluate the model's performance on a validation set.  
data/: Directory containing the dataset used for training and validation.  
README.md: This file, describing the project and setup. 

**Dependencies**  
To run this project, you need the following libraries:  
torch (PyTorch)
torchvision
numpy
matplotlib
pandas

**Model Overview**
VideoModel Class
The VideoModel class is composed of the following components:

1 CNN Encoder:  

A series of 2D convolutional layers to extract spatial features from each video frame.  
The network starts with a 3-channel input (RGB frames) and progressively increases the number of feature channels.  
After each convolutional layer, a BatchNorm2d and ReLU activation function are applied, followed by max-pooling to downsample the spatial dimensions.  

2 LSTM:  

After extracting features from each frame, the output is passed through an LSTM network to capture temporal dependencies between frames.
The LSTM has 256 hidden units and processes the sequence of frame features.

3 Fully Connected Layer:

The final output of the LSTM is passed through a fully connected layer (Linear) to classify the video into one of 10 possible classes.  

**Results**
After training, the model will output the final validation accuracy, which you can use to assess its performance. For more detailed results, you can adjust the training loop to log metrics.
