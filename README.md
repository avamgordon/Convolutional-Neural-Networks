# Convolutional-Neural-Networks
This repository showcases a programming project completed for CSE 5526 (Neural Networks) using PyTorch/Python to implement a CNN to train and test a handwritten digit recognition system using the MNIST dataset. 

The CNN architecture implemented is as follows in baseline(1).ipynb: 
- Inputs are reshaped to size 28x28 
- Two convolutional layers, where each convolution layer is followed by ReLU activation
- Six and tex 3x3 kernels, respectively, for the two layers using a stride of 1
- Softmax layer with 10 neurons for the output layer
- Xavier initialization based on uniform distribution
- Mini-batch gradient descent with momentum = 0.9 and mini batch size of 50
- Early stopping iwth a cross-entropy loss function
- Learning rate scheduler to adjust the learning rate by 10% every 10 epochs, starting with a learning rate of 0.05
- Training for 100 epochs
- An additional 3x3 max pooling layer after each convolutional layer, using a stride of 3 (added in baseline_pooling(1).ipynb)
- Adding in of dropout after each convolutional layer, using separate dropout rates of 0.25, 0.5, and 0.75, respectively (added in baseline_dropout(1).ipynb)
