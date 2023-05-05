# Agrculture_Image_Segmentation

This repository holds an attempt perform image segmentation task on the Agriculture Vision challenge. This challenge combines technique using Computer Vision, Data Science and AI/ML. https://www.agriculture-vision.com/agriculture-vision-2023

## Overview
The task is to use the dataset which are some aerial farmland images to train a model to predict field anomalies on new images. Given a new input from the test set our task is to predict what class does each pixel belong to (one of the six anomalies or the background).​The six anomalies are: Cloud shadow, Double plant, Planter skip, Standing Water, Waterway and Weed cluster. 

## Data
* Data:
  * Type: 
    * Input: the data set comes in zip file, and image file (.PNG)
  * Total size: ~20 GB.
  * The instances total of 21,061 aerial farmland images, each image consists of four 512x512 color channels, and they also has a boundary map and a mask. 
  * The boundary map indicates the region of the farmland, and the mask indicates valid pixels in the image. 
![image](https://user-images.githubusercontent.com/89665013/236540282-8d9fbd80-fdb1-4fc1-b71e-677141c23c6e.png)

  #### Preprocessing / Clean up

* Dealing with image data
* Masks data

### Problem Formulation

  * Input: ?
  * Output: ?
  * Models used: 
    * Deep Lab
    * UNet
    * UNet + fastai
    * UNet + VGG
