# Image-classifier-sign-or-number-
The project generates the images uses openCV in grayscale we can also generate RGB images. Then using the keras package I've build a convolutional neural network model then used that model to classify the images.

---
## Project Walkthrough 
First I've set up the hand histogram for skin tone. Then generated 400 images for every sign using the opencv. Then I've used the keras to train CNN model over the images and storing the model. Then using that model to predict the iamges
You'll need a lot of patience if you don't own a gpu. Training the model on CPU only takes around 4 hours for 10 epochs.

---

## Table of Contents
- Prerequisites
- How to work 
- Data Generation
- Modelling
- Prediction
- issues

---

## Prerequisites

numpy
os
tensorflow 1.5
keras
opencv 3.9 -python
pyttsx3

---
## Installation 

> $pip install 'Prerequisites'

install the Prerequisites one by one or place all of them in a text file and install

---
## How to work
Running the Code
Once We've installed all the prerequistes then we can open our cmd terminal and set the directory of the folder using 
 
 > $cd "path of the directory"
 
 ### Data Generation
 Then run the file to save the hist of the hand 
 
 > $python Data_generate-1-set_hand_hist.py
 
 once your hand covers the rectangles press "c" to see the grayscale version if you are satisfied then press "s" to save the hist.
 
 Then it comes to data Generation 
 
 > $python data_generate-2-create_gestures.py
 
 once you run the code then enter the gesture number and name after that there will be a webcam window with seprate a grayscale window. Once you are ready put your hand in the region of interest (the blue box). Then press "c". it will start capturing the images. You can pause or resume by pressing "c"
 
 ### Data Modeling
 
 It includes the CNN model. If you want to tweek the parameter then change the parameter. If you are using RGB images then change the input_shape=(50, 50, 1) change 1 to 3. Change the other inputs like activation function and cost function according to the data. then save it and run it in the cmd
 
 > $python Model-3-trainning.py
 
 ### Predictions 
 Run the final part of the project and get the predictions in the real time in the webcam window.
  
  >$python predictions_part-4.py
  
  ## Issues
  I've encountered certain issues with tensorflow and openCV as I don't had the GPU and not very powerfull CPU. I've installed tensorflow 1.5 because 2.0 version is not supported because of AVX. 
  I've followed these two links to get pass the issues . Hopefully I'll be helpfull
  >https://github.com/tensorflow/tensorflow/issues/36485  for tensflow 
  
  >https://stackoverflow.com/questions/54734538/opencv-assertion-failed-215assertion-failed-npoints-0-depth-cv-32 for openCV issues.
  
  ## Contact for any issues
  > Email - deepesh4194@gmail.com
