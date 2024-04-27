### Role of Activation Functions

Activation functions introduce non-linearity into our networks, allowing us to fit to non-linear data. If we just had simple linear things, we'd get 1 large linear combination of data. Rather, we can fit to more curved lines allowing for greater bias. 

### Differentiability and Quirks
- Activation functions must be chosen carefully because they can cause issues with vanishing gradients
- Sometimes they are not cont. diff. or cont. diffable
	- This causes issues in back propagation


### Common Activation Functions

Sigmoid

Softmax

ReLU

Leaky ReLU

