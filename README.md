# Image-classifier-sign-or-number-
The project generates the images uses openCV in grayscale we can also generate RGB images. Then using the keras package I've build a convolutional neural network model then used that model to classify the images.

---
### Project Walkthrough 
First I've set up the hand histogram for skin tone. Then generated 400 images for every sign using the opencv. Then I've used the keras to train CNN model over the images and storing the model. Then using that model to predict the iamges
You'll need a lot of patience if you don't own a gpu. Training the model on CPU only takes around 4 hours for 10 epochs.

---

### Table of Contents
- Prerequisites
- How to work 
- Data Generation
- Modelling
- Prediction
- issues

---

# Prerequisites

numpy
os
tensorflow 1.5
keras
opencv 3.9 -python
pyttsx3

---
# Installation 

> $pip install 'Prerequisites'

install the Prerequisites one by one or place all of them in a text file and install

# How to work
Running the Code
Once We've installed all the prerequistes then we can open our cmd terminal and set the directory of the folder using 
 
 > cd "path of the directory"
 
 #### Data Generation
 Then run the file to save the hist of the hand 
 
 > $python Data_generate-1-set_hand_hist.py
 
 once your hand covers the rectangles press "c" to see the grayscale version if you are satisfied then press "s" to save the hist.
 
 Then it comes to data Generation 
 
 > $python data_generate-2-create_gestures.py
 
 once you run the code there will be 
