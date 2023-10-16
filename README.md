# XOR Backpropagation Deep Learning

**Backpropagation** is a supervised learning algorithm used in training artificial neural networks, including multi-layer perceptrons (MLPs), to learn complex relationships between inputs and outputs. **XOR** (exclusive OR) is a classic binary classification problem that can be solved using a neural network trained with backpropagation.

## Artificial Neural Network (ANN) for XOR Problem

![image](https://github.com/kmnvz-mayvez/XOR-Backpropagation-deep-learning/assets/55338832/96d3c546-5c4e-40da-880e-d306618dea18)

The following figure illustrates an Artificial Neural Network (ANN) designed to tackle the Logical XOR problem. This ANN comprises:

- **2 input neurons** (u1, u2)
- **Bias neuron** (u0)
- **1 hidden layer** with **2 neurons** (u3, u4)
- **1 output neuron** (u5)

The activation function employed for each neuron (u3, u4, and u5) is the **sigmoid function**.

### Backpropagation Update

If the ANN is designed to solve the Logical XOR problem, you can update the weights (Wij) after **1 (ONE) EPOCH ONLY** using the backpropagation algorithm with a **learning rate h = 0.1**.

### Error Reduction

During this update, it's crucial to check if the error is reduced, as the objective of the backpropagation algorithm is to minimize the error and enhance the network's performance.

# Step-by-Step Guide

### Data Preparation

1. Define the XOR truth table, which has four data points: (0, 0), (0, 1), (1, 0), and (1, 1).
2. Label the output for each data point according to the XOR operation (0 XOR 0 = 0, 0 XOR 1 = 1, 1 XOR 0 = 1, 1 XOR 1 = 0).

### Network Architecture

3. Create a simple feedforward neural network. In this case, a network with one hidden layer containing two neurons and one output neuron will suffice.

### Initialization

4. Initialize the weights and biases randomly for all neurons in the network.

### Forward Pass

5. For each data point, perform a forward pass through the network by computing the weighted sum of inputs and applying an activation function (typically the sigmoid function or ReLU).
6. Calculate the output of the network.

### Calculate Error

7. Compute the error (the difference between the predicted output and the actual target) for each data point.

### Backpropagation

8. Update the network's weights and biases using the backpropagation algorithm. The backpropagation algorithm involves the following steps for each data point:
   - Compute the gradient of the error with respect to the output layer's weights and biases.
   - Compute the gradient of the error with respect to the hidden layer's weights and biases.
   - Update the weights and biases in the direction that minimizes the error using a learning rate and the computed gradients.

### Repeat Steps 4-6

9. Repeat the forward pass and backpropagation steps for multiple epochs until the network converges to a solution.

### Testing

10. After training, you can test the network by providing new input data to make predictions. Ensure that the network produces the expected XOR outputs for the given inputs.

### Fine-Tuning

11. Adjust hyperparameters like the learning rate and the number of hidden neurons if necessary to improve the network's performance.

This is a simplified example, and real-world problems may require more complex architectures and training techniques. Nevertheless, the backpropagation algorithm remains a fundamental concept in training neural networks. Keep in mind that, for XOR, a simple neural network as described above should be able to learn the function effectively.
