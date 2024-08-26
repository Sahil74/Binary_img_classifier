# Happy-Sad Image Classification

## Project Overview

- This project is a binary image classification model that distinguishes between two emotions: "Happy" and "Sad." 
The model is built using TensorFlow and Keras and is trained on a dataset of images labeled as either "Happy" or "Sad." 
The goal is to classify new images into one of these two categories.

## Code Structure

- Data Loading and Preprocessing: The code loads the dataset using TensorFlow's image_dataset_from_directory API.
                                  It then preprocesses the images by scaling the pixel values
                                  and splitting the dataset into training, validation, and test sets.
- Model Architecture: The model is a Convolutional Neural Network (CNN) with the following structure:
                      3 Convolutional Layers with ReLU activation and MaxPooling.
                      A Flatten layer to convert the 2D outputs into a 1D vector.
                      A Dense layer with 256 neurons and ReLU activation.
                      A final Dense layer with a sigmoid activation function for binary classification.
- Training: The model is compiled with the Adam optimizer and Binary Focal Crossentropy loss. It is trained for 20 epochs
            with a TensorBoard callback to log the training process.
- Evaluation: After training, the model's performance is evaluated using Precision, Recall, and Binary Accuracy metrics on the test dataset.
- Prediction: The script also includes a section for making predictions on new images.


## Model Training and Results

- Accuracy: The model achieved an accuracy of 100% on the training data and 100% on the validation data after 20 epochs.
- Loss: The training loss steadily decreased during training, with a final value of 0.0015. The validation loss also decreased,
        reaching a final value of 0.0011.

## Model Summary

## Conclusion

- This project demonstrates the application of a CNN for binary image classification. The model was able to classify images
with high accuracy, making it suitable for detecting emotions in images based on visual cues.
