flowchart TD
    A[Input Data x] --> B[Forward Pass: Weighted Sum + Activation]
    B --> C[Hidden Layers]
    C --> D[Output y']
    D --> E[Loss Function: Compare y' with True y]
    E --> F[Backward Pass: Compute Gradients]
    F --> G[Update Weights with Gradient Descent]
    G --> B
