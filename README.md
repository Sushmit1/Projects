## An Overview of my projects

1. Anime Face Generation using GANS :
     
   Trained a Deep Convolution GAN (DCGAN) on the Anime Face Dataset containing 63,000 images to generate Anime faces using PyTorch.
   Monitored the generator and discriminator losses throughout the training loop to ensure system progress and stability.
     
   Transition of Generated Images over 25 training epochs :
     
   After 1st Epoch:  
      ![alt text](https://github.com/Sushmit1/Projects/blob/main/Anime%20Face%20Generation%20using%20DCGAN/Generated/generated-image-0001.png)  
   After 10 Epochs:  
      ![alt text](https://github.com/Sushmit1/Projects/blob/main/Anime%20Face%20Generation%20using%20DCGAN/Generated/generated-image-0010.png)  
   After 25 Epochs:  
      ![alt text](https://github.com/Sushmit1/Projects/blob/main/Anime%20Face%20Generation%20using%20DCGAN/Generated/generated-image-0025.png)  

2. Dog Breed Identification Using Deep Learning :  

   Trained MobileNet-v2 CNN model on the Kaggle Dog Breed Identification Dataset containing 10,000 train and 10,000 test images comprising of 120 dog breeds using TensorFlow.
   Obtained a Multi-Class Log Loss Score of 0.92337 on the test data, demonstrating the model’s accuracy and robustness.

   Prediction from Trained Model:  
      ![alt text](https://github.com/Sushmit1/Projects/blob/main/Dog%20Breed%20Identification/imgs/output_with_truth_and_pred.png)
     
   Visualising Top 10 breeds for an image:  
      ![alt text](https://github.com/Sushmit1/Projects/blob/main/Dog%20Breed%20Identification/imgs/top_10_preds.png)

   Classify on Unknown User images :  
     ![alt text](https://github.com/Sushmit1/Projects/blob/main/Dog%20Breed%20Identification/user%20images/download%20(1).jpeg) ![alt text](https://github.com/Sushmit1/Projects/blob/main/Dog%20Breed%20Identification/user%20images/download%20(2).jpeg) ![alt text](https://github.com/Sushmit1/Projects/blob/main/Dog%20Breed%20Identification/user%20images/download.jpeg)

     ![alt text](https://github.com/Sushmit1/Projects/blob/main/Dog%20Breed%20Identification/imgs/user_imgs_preds.png)

3. Heart Disease Classification :

   On the UCI Heart Disease Dataset , trained and compared various models , chose the best performing model and tuned hyperparameters using both GridSearchCV and RandomizedSearchCV.  
   Obtained Accuracy of 84.79 % on the hyperparamter tuned LogisticRegression Model.

     ![alt text](https://github.com/Sushmit1/Projects/blob/main/Heart%20Disease%20Classification/metrics.png)


4. Housing Prices Prediction :
     
   Implemented a RandomForestRegressor through pipelines for Data Transformation and Model Training , producing a RMSE of 16259.24
