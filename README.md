# Contents
* LeNet





# LeNet
Hi today we discuss about the LeNet-5. it  was one of classic and very supper popular such as long time 
fist we discuss the architecture theoretically.
![LeNet-5](Architecture-of-LeNet-5-one-of-the-first-initial-architectures-of-CNN-Figure-from-29.png)

This the original image of LeNet-5 from research paper by Lechun eta al, 1998.

As LeNet-5 indicates there are 5 Layers with 2 Convolutional and three fully connected layers.Every convolutional layer has three parts such as Pooling Layer 
Convolution Layers,and Non-Linear activation function

LeNet start with input image as gray-scale image as from above figure we can see that 
the input has 
<img src="https://render.githubusercontent.com/render/math?math=32 \times 32 "> (bascially LeNet was build for MNIST data set)
and it passes through first convolutional layer and map  with 6
a filters of size <img src="https://render.githubusercontent.com/render/math?math=5 \times 5 "> with stride of 1.Then after this convoltional 
the dimension of image changes into <img src="https://render.githubusercontent.com/render/math?math=28 \times 28 \times 6"> and how we get converted this <img src="https://render.githubusercontent.com/render/math?math=32 \times 32 "> images into <img src="https://render.githubusercontent.com/render/math?math=28 \times 28 ">
is by pure arthimatics of input layer, which can be found using the formula below 

![](https://latex.codecogs.com/gif.latex?%5Cfrac%7Bn&plus;2p-f%7D%7Bs%7D&plus;1%20%5Ctimes%20%5Cfrac%7Bn&plus;2p-f%7D%7Bs%7D&plus;1)






# Reference
[![Research paper](http://yann.lecun.com/exdb/publis/pdf/lecun-01a.pdf)]