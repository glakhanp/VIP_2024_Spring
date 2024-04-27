
CNNs are similar to ANNs but involve a crucial convolution (generally implemented as cross correlation) and max pooling step.

The main idea behind convolution is to filter out various features from the supplied image and store it into a feature map. This feature map can then be used to make inferences on the features within the image (rather than the pixels themsleves). 
	- Filtering out features works by employing convolution, which takes into account general pixels to gather assumptions about the image

Once convolution has been applied to an image, CNNs will apply max pooling (or some sort of pooling step) where the image is partitioned into seperate chunks and further features are extracted.

Layers of [[Convolution]] and pooling can help CNNs isolate features and draw conclusions about the classification or regression task.

### Shrinking Size

A side effect of [[Convolution]] and pooling operations is that the size of the image to convolve/pool will generally decrease as layers are added.
- [[Convolution]] does not always go to the edge of the image (however there are cases in which techniques such as mirroring or wrap around can be employed to create a full feature map)
- Pooling often simplifies a partition into 1 value which can reduce the size of image into n pixels/partion area total values
