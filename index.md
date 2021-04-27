The goal of this project is to build a deep learning model that is able to correctly classify each pixel of the image. The **MSRC-v2 Dataset** was used for training and testing the model. It contains 591 Images and 23 different objects (classes). 
The Model consists of two parts: 

1. Encoder
2. Decoder

For Encoder was used the pre-trained mobilenet_v2. Only the downsampling layers were kept. Various architectures were tested for the decoder in order to find which delivers the better results. The final architecture of
the decoder consists of repeated Convolutional, Batch Normalization and Upsampling layers. ReLU turned out to be the most promising activation function in this case.

The final model delivered an accuracy of **82.79 %**

Results:

Given RGB photo: \
![alt text](Result-1.jpg)

and the Depth photo: \
![alt text](SS-Result-1.jpg)

PyTorch was used for the development of the model.
