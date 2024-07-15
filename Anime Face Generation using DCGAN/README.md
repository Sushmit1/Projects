## Anime Face Generation using DCGAN

Dataset : Kaggle Anime Face Dataset https://www.kaggle.com/datasets/splcher/animefacedataset containing 63,000 images of anime faces.  
  
Discriminator Network :  
- Inputs RGB images of 64 x 64 dimensions.
- Convolutional Blocks - The network employs a series of convolutional blocks, each consisting of the following elements :
    
  1. Convolution (Conv2d) Layer
  2. Batch Normalisation Layer :  Normalizes the activations of the previous convolutional layer across a mini-batch of data to stabilise training and converge faster.
  3. Leaky ReLU : Introduces a small non-zero slope for negative inputs, preventing the "dying ReLU" problem where gradients become zero.  
  
