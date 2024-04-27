Feedforward a series if inputs through a set of weights and biases that shape that input into some output.

### Standard Structure:

```
Input_Layer -> Hidden Layers -> Output Layer
```

### Activation Function Calculation
The input layer represents our first activations.
Activations in subsequent layers can be represented by this formula where the activation neuron at index j, in layer L is the weighted sum of the neurons in the previous layer through some [[Activation Functions]] g. 

### Activation Formula
$a_j^L = g(\sum_{k=0}^{n}w_{kj}^L*a_k^{L-1})$

Weights are randomly initialized upon neural network creation and updated through the process of gradient descent and backpropogation to minimize the [[Cost Functions]] and maximize the neural network's ability to correctly make inferences. 





