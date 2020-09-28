# Face_mask_detection_transferlearning

This project is a part of the CNN Deep learning using transfer learning(Resnet152) and Opencv.

#### -- Project Status: [Completed]

## Project Intro/Objective
The purpose of this project is to detect whether person has wear mask or not.

### Methods Used
* Data gathering
* Data preprocessing
* Build CNN model(use Resnet152)
* Model evaluation
* Predictive Modeling

### Technologies
* Python
* jupyter
* Numpy 
* Matplotlib
* tensorflow>=2.1.0
* keras==2.3.1
* Resnet152
* Opencv

## Project Description
This is project based on transfer learning(Restnet152) CNN model. 
Dataset used by this project is 'https://drive.google.com/drive/folders/1P3gIgFUMbdl5tSqx1pK385bz4t0mxEvW?usp=sharing'. Dataset conatins train, test and validation data in each there are two class 'with_mask' and 'without_mask'. After downloading and importing dataset(in Google colab) i used 'Resnet152' model to train my model.

Resnet architecture.

<img src='https://github.com/vishalbarad/Face_mask_detection_transferlearning/blob/master/The-basic-architecture-of-Resnet152.png'>

After that i just use 'model checkpoint' callback function to save best model as 'Face_mask_scratch.h5'.

Face_mask_detection using transferlearning 'https://github.com/vishalbarad/Face_mask_detection_transferlearning')

After that i just compile model using 'Adam' optimizer with learning rate=0.01, loss='categorical_crossentropy'.

After that i did data image augmentation like rescale image, rotate image, flip image, zoom image etc.

#### **Data Augmentation**: It is a way to generate more training data frm our currenet set. It augments the training data by generating new eg via random transformation of existing ones. This way we artificially boost the size of the training set, reducing overfitting.

After that i just fit data using 10 epochs.

At the end i got 87% validation accuracy and 87% training accuracy.

Then again i just saved model as 'Face_mask.h5' (Model is >200mb so you can download from this link https://drive.google.com/file/d/1WdGiJbE3KJpEVA38I3aEK64DaN74gtIj/view?usp=sharing.)

After downloading model i made 'prediction.ipynb' file using Opencv to predict output.

## Needs of this project

- frontend developers
- data exploration/descriptive statistics
- data processing/cleaning
- writeup/reporting

## Contact
* Feel free to contact me any questions or if you are interested in contributing!


<h1 align=center>Thank You</h1>

