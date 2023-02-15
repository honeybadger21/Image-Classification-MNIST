# ImageClassificationMNIST

The goal of this assignment is to create a neural network that has greater than 99% accuracy on the MNIST dataset. Training and Model Saving was accomplished using Google Collab. Webpage creation and model deployment was done through Anvil. Link to the webpage: https://msbaoptim38.anvil.app/

About the Dataset: The MNIST Handwritten Digits Dataset is considered as the “Hello World” of Computer Vision. Most standard implementations of neural networks achieve an accuracy of ~(98–99) percent in correctly classifying the handwritten digits. The MNIST dataset consists of 60,000 training examples and 10,000 examples in the test set.

Details of the Model Used: Instead of building a model from scratch, LeNet-5 (LeCun et al., 1998. Gradient based learning applied to document recognition) convolutional neural network was taken as the baseline standard model. It’s a simple model consisting of a convolutional layer with a max-pooling layer twice followed by two fully connected layers with a softmax output of ten classes at the end. After training for 30 epochs, the training accuracy was 99.98% & dev set accuracy was 99.05%. For a model released in 1998, the accuracy seems pretty good.

However, the model suffers from both high variance and high bias problems with a test set accuracy lower than 98.74%. Let us tackle both the problems one by one. We tackle these issues as follows: For Reducing Variance: Data Augmentation, L2 Regularization, DropOut Regularization, Batch Normalization, Variable Learning Rate. For Handling Bias: More Layers, Deeper Network.

To summarise, we are using two convolutional layers, followed by a pooling layer twice (once with 32 filters and 64 filters respectively) and three fully connected layers with a softmax unit in the end with 10 classes. Batch Normalization, L2 Regularization and Dropouts are done in-between the layers.
