## Dog Breed Identification using Deep Learning 

- Dataset was used from the Kaggle Dog Breed Identification competition https://www.kaggle.com/competitions/dog-breed-identification which contains 10,000 train and 10,000 test images of 120 breeds of dogs.
- The Evaluation Metric was Multi Class Log Loss between the predited probability and the observed target.

### Deep Learning Model Used : Mobilenet V2 fitted on the training data.

The model is composed of the following layers:  
1. Input Layer: Uses the pre-trained MobileNetV2 model from TensorFlow Hub.  
2. Output Layer: A dense layer with a softmax activation function to classify images into the specified number of categories.
