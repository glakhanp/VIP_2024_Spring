Recurrent Neural Networks let us take in a variable number of inputs and map them to a variable number of outputs.

The general RNN architecture involves taking one series of layers and "unrolling them." Unrolling is when we use the same layer for each input and feed the output for each input foward.

This allows the RNN to operate on information earlier on in the sequence. 

It's important to note that an RNN has multiple activation functions. One before being output to the next time step, and one for the output of an rnn layer. 

### VGP for RNNs

One major issue with traditional RNNs is the vanishing gradient problem. Earlier values in the sequence are subject to many multiplications during backpropogation. Moreover since weights are shared during backpropogation, if the weight is less than 1 or vice versa, we can increase the chances of earlier gradients vanishing or exploding.

For this reason architectures such as GRU or LSTM were created which would help retain earlier information. 