***Coastline Detection through Image Segmentation using UNet***
Authors: Donovan Dahlin, Kristine Veneles
Mentors: Dr. Dulal Kar, Jacob Hopkins

***Research Goal***
Create a Convolutional Neural Network that can detect water at shoreline in order to track coastline. 
Architecture used is UNet proposed by Olaf Ronneberg
VGG16 is used as the pre-trained model for transfer learning to train model faster, provided by Keras. 

***Dependencies***
tensorflow 2.1.0
keras 2.3.1
segmentation-models 1.0.1
numpy 1.20.2
matplotlib 3.3.4
python 3.7.10
opencv 3.4.2

***Environment Set-up***
Jupyter Lab via Anaconda
GPU: NVIDIA GeForce RTX 2070 SUPER

***Data Set-up***
Folder name 'data' has 6 folders:
image names corresponds with masks
 - train_img
 - train_mask
 - test_img
 - test_mask
 - valid_img
 - valid_mask
 ---- Masks were created using LabelMe ----
 - LabelMe from Github creates annotated masks
     source: https://github.com/wkentaro/labelme
 - Annotated Masks were transformed to PNG file via GitHub source
     source: https://github.com/pei223/labelme_json_to_png
     
***Video Files Used***
cape_cod_edit.mp4
bob_hall_pier.mp4
 ---- Frames were retrieved and used as the images for train, test, valid ----
   -- Other images of shorelines collected from pixabay 

***ShorelineDetection Folder within KristineVeneles***
ShorelineDetection Folder consists of the jupyter notebook, 
data and the folder where the model is saved.