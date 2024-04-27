
When we use non-linear activation functions such as sigmoid or tanh, extreme values have gradients that are essentially 0. This means that even very large changes earlier in the network, or later in the network have little to no meaning on the actual value. Our gradients become basically 0 and training will sort of come to a halt. 

