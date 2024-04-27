
Sigmoid leads to issues with vanishing gradients because extreme values will have gradients of zero, so if we mess up the initial weights we could have extremely slow updates to our weights.

Moreover if our activations ever get too large, we could run into the same vanishing gradient issue. 

