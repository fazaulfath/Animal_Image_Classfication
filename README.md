# Animal Classification Project

## Overview
This repository provides a solution for classifying animals using transfer learning with a pre-trained VGG16 model. The project is designed to be executed in Google Colab and leverages TensorFlow and Keras to process images, build a classification model, and perform predictions on new data. The model is trained to distinguish between 15 different animal classes.

## Requirements
Google Colab: The repository is intended for use in Google Colab, which offers the necessary computing environment and pre-installed libraries.
Dataset: A zipped file containing images organized into folders (one folder per animal class). The expected structure is that each class folder is located inside a main dataset folder.
Libraries: TensorFlow, Keras, Matplotlib, and Scikit-learn (all available in Colab).

## How to Use This Repository
### Open the Notebook in Google Colab:
Launch the provided notebook from this repository in your Google Colab environment.

### Upload and Extract the Dataset:
Use the upload widget provided in the notebook to upload your zipped dataset file. The notebook will automatically extract the contents into the appropriate directory structure.

### Preprocess the Data:
The notebook sets up an image data generator that normalizes image pixel values and splits the dataset into training and validation sets (80% training and 20% validation).

### Build and Train the Model:
A VGG16 model (pre-trained on ImageNet) is used as the base for the network, with additional fully connected layers added on top for the classification of 15 animal classes. Run the training cells to train the model for the specified number of epochs.

### Evaluate the Model:
Once training is complete, the notebook evaluates the model on the validation set. It reports accuracy and generates a confusion matrix to help you understand how well the model is classifying the images.

### Predict on New Images:
The notebook includes a section where you can upload a new image, and the model will predict its class based on the training it received.

## Results
During training, progress is displayed with training and validation metrics. In a sample run, the model reached a validation accuracy of approximately 60%. A confusion matrix is generated at the end of training to provide insights into the performance across the different animal classes.

