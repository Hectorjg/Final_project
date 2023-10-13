# Project: Image classification of x-ray pneumonia
 
The goal is to predict as accurately as possible if the chest x-ray image shows pneumonia or if it is normal.
The model is a CNN of deep learning.
The dataset used for this project can be found on www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia/data

## Objectives
  - Understand the information (image size, colors, size of the dataset, classes).
  - Build the architecture of the model considering the nature of the information.
  - Understand the plots to improve the model.
  - Test the model and save it.

## Project Steps:

### Data pre process
  - Load the dataset and select the colors (Gray scale or RGB).
  - Resize the images.
  - Define the callbacks.
  
### Data Analysis
  - Check for imbalance in the data.
    
### Processing Data
  - Data augmentation.
  
### Building the model
  - Using Sequential() as a model.
  - 1 Conv2D(32), 2 Conv2D(64), 1 Conv2D(128), 1 Convd2D(256), Flatten, 2 Dense (128, 64), Output.
  - Choose the Output Activation.
  
### Compile to train the model
  -Select the optimizer.
  
  -Choose the Loss metrics.
  
  -Choose the accuracy metrics.
  
### Evaluate Accuracy
  - Accuracy.
  - F1-score.
  - Precision.
  - Recall.
  - Plot of the Loss in train and val.
  - Model.predict() on test set.
  
## Conclussion:

  -The Learning rate of the model is slow, meaning that the model has problems converging.
  -Even if the accuracy archives a 92.30% accuracy, it might need a deeper architecture to perform better.

   --------------------------------
   Model: cnn_92.joblib
   --------------------------------

   ## Aditional dataset: Diabetic retinopathy
  - This is a CNN model for a multiclass classification problem with 5 different classes.
  - This dataset has all the images in the same size, but the number images per class is imbalanced.
  - The architecture may be similar to the architecture of "pneumonia", but all the parameters are different due to the nature of the images.
  - The dataset can be find in: www.kaggle.com/datasets/sachinkumar413/diabetic-retinopathy-preprocessed-dataset.
