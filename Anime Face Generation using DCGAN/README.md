## Anime Face Generation using DCGAN

Dataset : Kaggle Anime Face Dataset https://www.kaggle.com/datasets/splcher/animefacedataset containing 63,000 images of anime faces.  
  
Discriminator Network :  
- Inputs RGB images of 64 x 64 dimensions.
- Convolutional Blocks - The network employs a series of convolutional blocks, each consisting of the following elements :
    
  1. Convolution (Conv2d) Layer with increasing output channels (64 → 128 → 256 → 512)  
  2. Batch Normalisation Layer :  Normalizes the activations of the previous convolutional layer across a mini-batch of data to stabilise training and converge faster.
  3. Leaky ReLU : Introduces a small non-zero slope for negative inputs, preventing the "dying ReLU" problem where gradients become zero.
       
- Output Layer :
  The final convolutional layer has 1 filter, effectively compressing the high-dimensional feature maps into a single value per image.  
  Flatten: Reshapes the multi-dimensional output from the previous layer.  
  Applies the sigmoid activation function, which maps the output values between 0 and 1, enabling probabilistic interpretation.  
