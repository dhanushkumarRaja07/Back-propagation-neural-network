Backpropagation is the learning algorithm used in artificial neural networks. It is based on the principle of gradient descent and the chain rule of calculus.
Perform a forward pass and calculate predictions.

Compute the loss between predictions and actual labels.

Start from the output layer:

Calculate gradient of loss w.r.t. outputs.

Propagate gradients backward through each hidden layer using the chain rule.

Compute gradients for all weights and biases.

Update weights using gradient descent.

Repeat for many epochs until the loss converges.

flowchart TD
    A[Input Data x] --> B[Forward Pass: Weighted Sum + Activation]
    B --> C[Hidden Layers]
    C --> D[Output y']
    D --> E[Loss Function: Compare y' with True y]
    E --> F[Backward Pass: Compute Gradients]
    F --> G[Update Weights with Gradient Descent]
    G --> B
