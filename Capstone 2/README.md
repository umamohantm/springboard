
# Abnormality detection in bone X-Ray radiographs 


# Overview

Bio-medical image analysis is an interdisciplinary field which includes: biology, physics, medicine and engineering. It deals with application of image processing techniques to biological or medical problems. Medical images to be analyzed contain a lot of information regarding the anatomical structure under investigation to reveal valid diagnosis and thereby helping doctors to choose adequate therapy. Doctors usually analyse these medical images manually through visual interpretation.

# Goals

Diseases and injuries to the bone are the major contributing factors in causing abnormalities in bones. Whenever there is an injury to the bone, the physician asks you to do an X-Ray, thus when such hundreds of patients visit hospitals everyday there are massive numbers of X-rays done on a regular basis. To be specific with the stats, Musculoskeletal conditions affect more than 1.7 billion people worldwide, and are the most common cause of severe, long-term pain and disability, with 30 million emergency department visits annually and increasing. So, in order to reduce the error rate of the Radiologist and to do the analysis much faster, an AI solution should suffice the purpose. 

# DataSet

Dataset used in this project is called MURA. MURA is one of the largest public radiographic image datasets. MURA is a dataset of musculoskeletal radiographs consisting of 14,863 studies from 12,173 patients, with a total of 40,561 multi-view radiographic images. Each belongs to one of seven standard upper extremity radiographic study types: elbow, finger, forearm, hand, humerus, shoulder, and wrist. You can download the dataset from the official contest website here. https://stanfordmlgroup.github.io/competitions/mura/

## The steps involved in this project are below ,
### Data Wrangling : <br>
The data originally obtained was in CSV file and directly loaded into the pandas data frame. The data is relatively clean so need of data cleaning. <br>
### EDA : <br>
Having an Imbalanced Dataset? This is checked in this step. The training and validation datasets are having balanced data. 
### Preprocessing : <br> 
Using OpenCV library image is enhanced. First the image contrast is increased using Contrast Limited Adaptive Histogram Equliser (CLAHE).For detecting the edges cv2.canny() is used.After detecting the edges the original image is cropped based on the dimensions obtained by detecting the edges of the original image. For blurring and smoothing the image cv2.GaussianBlur() is used.<br>

## Before and After Image Enhancement<br>
![Image](https://github.com/umamohantm/springboard/blob/master/Capstone%202/data/Before_and_after.PNG)<br>
<br>
Image augumentation is done using ImageDataGenerator from Keras

