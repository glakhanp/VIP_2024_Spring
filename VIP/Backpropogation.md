Backpropogation is the process of updating the weights and biases of the neural network to better fit the data and make inferences. 

It involves minimizing the cost function through a process called gradient descent where the neural network will calculate the partial derivative of the cost function with respect to each weight and update them accordingly to find the weights where the cost is lowest. 

Backpropogation involves extended use of the chain rule. 

### Role of summing derivatives for previous layers 

- When we are calculating the partial derivate with respect to an earlier weight in the network, we need to factor in its effect on a neuron that effects later layers in the network. This requires us to, when carrying out chain rule, to sum up all the change across all the later neurons and weights the earlier neuron can affect. This appears as taking the derivative with respect to that neuron, and then the derivative of that neuron with respect to its weight (which ofc becomes the earlier activation).
	- Doing this is a tedious and time consuming process (BTW)
	- Matrix methods can speed this up significantly
