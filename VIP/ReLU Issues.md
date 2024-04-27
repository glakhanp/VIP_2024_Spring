
ReLU can lead to exploding gradients if our intialization values are too large. This happens because the weights will make the values too large and in our backprop pass we'll get gradients that essentially explode. 

ReLU due to it zeroeing out for negative values mean that values will not change for that neuron when gradients are updated. This in a sense causes the neuron to die because it won't get updated and will keep outputting 0 as a result. 

Leaky ReLU was then created to give the neuron a chance to recover by allowing very small changes to the negative value and letting it become positive as training continued. 

ReLU is not cont. diffable

This means that we have to use an if statement to compute relu. 



