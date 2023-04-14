# OSS4009CoputerVision
Dangerous and suspicious human pose detection using skeleton pose

Institution: Carleton University

Course: OSS4009 Computer Vision 

Term: W23

Students: Adam Thompson, Philippe Beaulieu

Professor:  Dr. Marzieh Amini

Description:

Camera hardware needed: regular webcam
 
These programs will take the stream of a webcam and predict a defined human pose which is classified as safe or dangerous
(all non-dangerous pose are safe). All the codes are present to create the dataset from images, train the model, 
and then be able to predict the human pose with a live feed from a webcam (or other image capturing devices).
              
 Files (to be executed in order if you don't have the dataset):
 - 0 - Pre1 - csv_dataset_creation.ipynb, to create the mediapipe landmark dataset
 - 0 - Pre2 - cnn_model_creation.ipynb, to create the CNN trained model
 - 1 - MAIN - Dagerous_Skeleton_Pose_Detection.ipynb, main program to predict the gesture
 - class_name.json, class name from the categogies
 - dataset3.csv, Mediapipe landmark dataset
 - model.tflite, CNN trained model (not included as file is too large)
 
  The folder hierarchy is important to load the images, it is as follow:

     DATASET
       -TRAIN
          -folder0
             - image0.jpg
             - image1.jpg
             - image2.jpg
             - ...
          -folder1
             - image0.jpg
             - image1.jpg
             - image2.jpg
             - ...
          -...
       -TEST
          - image0.jpg
          - image1.jpg
          - image2.jpg
          - ...
