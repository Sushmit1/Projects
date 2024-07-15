## Anime Face Generation using DCGAN

Dataset : Kaggle Anime Face Dataset https://www.kaggle.com/datasets/splcher/animefacedataset containing 63,000 images of anime faces.  
  
## Discriminator Network :  
- Inputs RGB images of 64 x 64 dimensions.
- Convolutional Blocks - The network employs a series of convolutional blocks, each consisting of the following elements :
    
  1. Convolution (Conv2d) Layer with increasing output channels (64 → 128 → 256 → 512)  
  2. Batch Normalisation Layer :  Normalizes the activations of the previous convolutional layer across a mini-batch of data to stabilise training and converge faster.
  3. Leaky ReLU : Introduces a small non-zero slope for negative inputs, preventing the "dying ReLU" problem where gradients become zero.
       
- Output Layer :
  The final convolutional layer has 1 filter, effectively compressing the high-dimensional feature maps into a single value per image.  
  Flatten: Reshapes the multi-dimensional output from the previous layer.  
  Applies the sigmoid activation function, which maps the output values between 0 and 1, enabling probabilistic interpretation.  

## Generator Network :
  - Inputs a Latent Vector (random noise vector) of size 128 and initial dimensions of this noise vector is 1x1.  
  - Deconvolution Blocks :  
    1. Perform Transposed Convolution Function , the opposite operation of Convolution decreasing the ouput channels (512 → 256 → 128 → 64)
    2. Batch Normalisation Layer
    3. ReLU Activation Function to introduce non-linearity into the network.
  - Output Layer :
    The final deconvolutional layer has 3 filters, corresponding to the three color channels (RGB) of the generated image.  
    The output dimensions are expected to be 64x64 pixels, matching the desired image size.  
    Tanh Activation function to map the output values between (-1 and 1) , due to normalisation of images at the image pre-processing step.

Below is the Transition of the Generated images over 25 epochs :  

After 1st Epoch:  
      ![alt text](https://github.com/Sushmit1/Projects/blob/main/Anime%20Face%20Generation%20using%20DCGAN/Generated/generated-image-0001.png)  
   After 10 Epochs:  
      ![alt text](https://github.com/Sushmit1/Projects/blob/main/Anime%20Face%20Generation%20using%20DCGAN/Generated/generated-image-0010.png)  
   After 25 Epochs:  
      ![alt text](https://github.com/Sushmit1/Projects/blob/main/Anime%20Face%20Generation%20using%20DCGAN/Generated/generated-image-0025.png)  
