## Dog Breed Identification using Deep Learning 

- Dataset was used from the Kaggle Dog Breed Identification competition https://www.kaggle.com/competitions/dog-breed-identification which contains 10,000 train and 10,000 test images of 120 breeds of dogs.
- The Evaluation Metric was Multi Class Log Loss between the predited probability and the observed target.

### Deep Learning Model Used : Mobilenet V2 fitted on the training data.

The model is composed of the following layers:  
1. Input Layer: Uses the pre-trained MobileNetV2 model from TensorFlow Hub.  
2. Output Layer: A dense layer with a softmax activation function to classify images into the specified number of categories.

### Result : Obtained a Multi-Class log loss score of 0.92337

Prediction from Trained Model:  
      ![alt text](https://github.com/Sushmit1/Projects/blob/main/Dog%20Breed%20Identification/imgs/output_with_truth_and_pred.png)
     
   Visualising Top 10 breeds for an image:  
      ![alt text](https://github.com/Sushmit1/Projects/blob/main/Dog%20Breed%20Identification/imgs/top_10_preds.png)

   Classify on Unknown User images :  
     ![alt text](https://github.com/Sushmit1/Projects/blob/main/Dog%20Breed%20Identification/user%20images/download%20(1).jpeg) ![alt text](https://github.com/Sushmit1/Projects/blob/main/Dog%20Breed%20Identification/user%20images/download%20(2).jpeg) ![alt text](https://github.com/Sushmit1/Projects/blob/main/Dog%20Breed%20Identification/user%20images/download.jpeg)

![alt text](https://github.com/Sushmit1/Projects/blob/main/Dog%20Breed%20Identification/imgs/user_imgs_preds.png)
