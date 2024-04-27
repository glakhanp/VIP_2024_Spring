Skip connections work by feeding forward the input to the next layer. 

What this does is allow the network to learn the difference between an input and its output. So instead of having to learn the function taht maps the input to the output it only learns the difference.

This is helpful because adding many layers can make it difficult for a model to learn the identity of a function. So if earlier layers converge and figure out an optimal solution, later layers will have to train to propogate the earlier signal forward.

However learning an identity function for a neural network is a little difficult and so later layers simply add noise to the output and degrade accuracy. They also have the effect of contributing to gradient problems and making training more difficult.

Skip connections work by directly connecting earlier neurons/actuvations to later ones, which essentially causes the model to learn the difference between the input and output.

This for one makes it easier for the model to learn the identity mapping of a function and so if a model figures things out earlier in the network, later layers will be able to more easily propogate the signal forward and with less noise.

So resnet allows for deeper networks without causing the addition of noise.

Another benefit of resent is mitigating the vanishing gradient problem... but how?

Also how do we connect larger layers to smaller ones?
- Look into this

One thing to note is that sometimes the input and output dimensions don't match in which case they perform 1x1 convolution. 