![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![Google Cloud](https://img.shields.io/badge/GoogleCloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white)![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1AHJIH6x8JwlPKIOW6J6YovJjs8BUjfMQ?authuser=1#scrollTo=OGdKitdexmid)





# LeNet
 Today we discuss about the LeNet-5. it  is one of classic and very supper popular such as long time 
fist we discuss the architecture theoretically.
![LeNet-5](Architecture-of-LeNet-5-one-of-the-first-initial-architectures-of-CNN-Figure-from-29.png)

The above diagram shows a description of the LeNet-5 architecture as shown in the original document.

**Layer 1-** The first layer is the input layer; It is generally not considered a layer of the network as nothing is learned on that layer. The input layer supports 32x32, and these are the dimensions of the images that will be passed to the next layer.

The grayscale images used in the research paper had their pixel values normalized from 0 to 255, to values between -0.1 and 1.175. The reason for normalization is to ensure that the batch of images have a mean of 0 and a standard deviation of 1, the benefits of this is seen in the reduction in the amount of training time. In the image classification with LeNet-5 example below, we’ll be normalizing the pixel values of the images to take on values between 0 to 1.

**Layer 2-** Layer C1 is a convolution layer with six 5 × 5 convolution kernels, and the feature allocation size is 28 × 28, whereby input image information can be avoided.

**Layer 3-** Layer S2 is the undersampling / grouping layer which generates 6 function graphs of length 14x14. Each cell in every function map is attached to 2x2 neighborhoods at the corresponding function map in C1.

**Layer 4 -** C3 convolution layer encompass sixteen 5x5 convolution kernels The input of the primary six function maps C3 is every continuous subset of the 3 function maps in S2, the access of the following six function maps comes from the access of the 4 continuous subsets and the input for the following 3 function maps is crafted from the 4 discontinuous subsets.Finally, the input for the very last function diagram comes from all the S2 function diagrams.

**Layer 5-** Layer S4 is just like S2 with a length of 2x2 and an output of sixteen 5x5 function graphics.

**Layer 6-** Layer C5 is a convolution layer with one hundred twenty convolution cores of length 5x5. Each cell is attached to the 5x5 neighborhoods along sixteen S4 function charts. Since the function chart length of S4 is likewise 5x5, the output length of C5 is 1 * 1, so S4 and C5 are absolutely linked.

It is referred to as a convolutional layer in preference to a completely linked layer due to the fact if the input of LeNet-5 becomes large and its shape stays unchanged, then its output length is bigger than 1x1, i.e. now no longer a completely linked layer.

**Layer 7-** The F6 layer is connected to C5 and 84 feature charts are generated. In the grayscale images used in the research, the pixel values ​​from 0 to 255 were normalized to values ​​between -0.1 and 1,175 The reason for normalization is to make sure the image stack has a mean of 0 and a standard deviation of 1.


# Reference
