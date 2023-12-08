# Pizza_or_Pizzanot

Binary Classifier Neural Network Documentation

This documentation provides an overview of the implementation of a binary classifier using a neural network with the PyTorch library on Google Colaboratory. The classifier distinguishes between images of pizzas and non-pizzas, achieving an accuracy of 83% on a test dataset.

Data Loading and Preprocessing

Mount Google Drive:

The Google Drive is mounted to access the dataset.
Load and Display Images:

Images from the 'pizza' and 'not_pizza' directories are loaded using mpimg and converted into PyTorch tensors.
Dataset Splitting:

The dataset is split into training and testing sets, with 500 and 100 samples, respectively.
Data Reshaping:

Images are reshaped into vectors, and pixel values are normalized to the range [0,1].
Labeling:

Binary labels (1 for pizza, 0 for not pizza) are assigned to training and testing samples.


Neural Network Architecture

Define Neural Network:

A neural network with two hidden layers (10 and 12 nodes) and a logistic regression output layer is defined using the Sequential API.

Activation Functions:

ReLU activation functions are applied to hidden layers, and a Sigmoid activation function is used for the output layer.

Model Check:

The model is tested on a sample to verify its functionality.
Training the Model

Loss Function:

Binary Cross Entropy Loss is used as the loss function.
Training Loop:

The model is trained for 10,000 iterations with a learning rate of 0.005.

Save Model:
The trained model is saved as 'model_best.pt.'

Model Evaluation

Prediction on Test Data:
The model is tested on a sample from the test dataset, and the prediction is displayed along with the corresponding image.

Accuracy Calculation:
The predict function calculates and prints the accuracy on both the training and test datasets.
Results

Results Summary:
The model achieves 100% accuracy on the training set and 83% accuracy on the test set.

Conclusion:
The neural network effectively classifies pizza and non-pizza images, demonstrating the successful implementation of a binary classifier using PyTorch on Google Colaboratory.
