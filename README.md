# Video Classification with CNN and LSTM
This project implements a video classification model using a combination of Convolutional Neural Networks (CNN) and Long Short-Term Memory (LSTM) networks. The model is designed to take video frames, extract spatial features using a CNN, and process temporal dependencies between frames using an LSTM. The final output is a classification of the video into one of 10 classes.

Project Structure  
VideoModel.py: Contains the implementation of the VideoModel class, which is used for video classification.  
train.py: The script to train the model.  
evaluation.py: Code to evaluate the model's performance on a validation set.  
data/: Directory containing the dataset used for training and validation.  
README.md: This file, describing the project and setup.  
Dependencies  
To run this project, you need the following libraries:  

torch (PyTorch)
torchvision
numpy
matplotlib
pandas
