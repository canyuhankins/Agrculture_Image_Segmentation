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
![image](https://user-images.githubusercontent.com/98187543/236552184-1949db0e-deaf-430e-b485-67d557d8921a.png)

 #### Data Visualization
  * Example:
  
![image](https://user-images.githubusercontent.com/98187543/236550315-ff3f7465-7d15-4715-a3b5-7e7b56aceb8c.png)
![image](https://user-images.githubusercontent.com/98187543/236550391-856061a0-ce5a-4eec-a998-91abd9f7550c.png)


### Problem Formulation

  * Input: Overhead image of plots of lands. Image data, masks data convert into list of arrays
  * Output: Mask of plots of land
  * Models used: 
    * Deep Lab
    * UNet
    * UNet + fastai
    * UNet + VGG
* Deep Lab:


* UNet:

Unet is a CNN architecture originally designed for use of image segmentation utilizing medical scans. It consists of encoding and decoding layers. The econding layers reduce the size of the image while to decoding layers follow the same typical architecture of a CNN.

![image](https://user-images.githubusercontent.com/98187543/236554037-9534a58a-bf52-48c6-9f4d-1480512218bf.png)


### Model Results

  * DeepLab

 ![image](https://user-images.githubusercontent.com/89665013/236551019-ad66839e-55b8-4f09-b04d-042a305d683a.png)
 ![image](https://user-images.githubusercontent.com/89665013/236551126-23bda62c-97e0-4bb9-9bcc-5d6a14205bd0.png)
 ![image](https://user-images.githubusercontent.com/89665013/236551238-f4571b03-59fd-4b7c-b796-9a19303d9b5b.png)
 
  * Unet

![image](https://user-images.githubusercontent.com/98187543/236554943-5f1531cb-ba17-477f-89dc-a5e593fb154b.png)
![image](https://user-images.githubusercontent.com/98187543/236555114-1ff23906-f3ec-4810-806a-f8b605d1a7ff.png)





### Performance Comparison

* The metric is Mean Intersection-over-Union (mIoU)):
![image](https://user-images.githubusercontent.com/89665013/236550741-2bd5505f-1f35-4b41-9ef3-1e9377097ebd.png)
![image](https://user-images.githubusercontent.com/89665013/236550787-05da44d1-a6d9-4428-87d9-91f850ee3491.png)
