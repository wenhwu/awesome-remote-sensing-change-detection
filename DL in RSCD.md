# Deep learning in remote sensing change detection

## 1. why the CNNs commonly used is not possible in remote sensing change detection task?

A direct use of CNNs commonly used in typical recognition tasks, e.g., [AlexNet](https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf), [VGG Nets](https://arxiv.org/abs/1409.1556), and [GoogLeNet](https://arxiv.org/abs/1409.4842), is not possible in our task, as we believe that a simpler network architecture is more appropriate for our problem due to the following reasons:

* First, change detection aims to distinguish only several classes (two for binary change detection), which requires much less model complexity than general visual recognition problems in computer vision, such as ImageNet classification with 1,000 categories.
* Second, since spatial resolution of multispectral imagery is limited, it is desirable to make input size small, which reduces the depth of the network naturally.
* Third, a smaller network is obviously more efficient in change detection problems, where testing may be performed in a large-scale area.
* Finally, the above-mentioned networks are not suitable to be used on multispectral images with a large number of spectral channels.

**Reference**

[Learning Spectral-Spatial-Temporal Features via a Recurrent Convolutional Neural Network for Change Detection in Multispectral Imagery](https://arxiv.org/abs/1803.02642)
