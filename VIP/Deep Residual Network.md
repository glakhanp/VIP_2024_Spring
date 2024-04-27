
In traditional conv. neural networks (ie vgg) the initial signal has a hard time being carried through because weights in layers are initialized close to 0 meaning that it's easy for the signal to get lost.

Series of these layers and activation functions can make our output a garbled mess so to speak.

So residual connections which pass through the original signal along with some learned value were introduced. This means that the network can learn the difference between the input and output, rather than trying to learn the harder task of preserving the input signal.

This is done by passing the data forward. 

