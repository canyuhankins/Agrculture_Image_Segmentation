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
* Preprocessing involved going through each of the labels and combining all the masks together with each pixel referencing a different label.
* After combining the masks together, the next step was to associate each mask with the appropriate image.
  * Example:
  
![image](https://user-images.githubusercontent.com/98187543/236550315-ff3f7465-7d15-4715-a3b5-7e7b56aceb8c.png)
![image](https://user-images.githubusercontent.com/98187543/236550391-856061a0-ce5a-4eec-a998-91abd9f7550c.png)


### Problem Formulation

  * Input: Overhead image of plots of lands
  * Output: Mask of plots of land
  * Models used: 
    * Deep Lab
    * UNet
    * UNet + fastai
    * UNet + VGG


### 
