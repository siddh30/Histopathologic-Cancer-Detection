#  <div align="center"> Histopathologic Cancer Detection </div>

<p align = "center"><img width="500" img height="100" src = "https://github.com/siddh30/Histopathologic-Cancer-Detection/blob/master/logo.png"</p>


The goal of this project is to create an algorithm that will identify the metastatic tissues in histopathologic scans of the lymph node sections using one of the deep learning techniques – Convolutional Neural Network. We aim to classify cancer tissues based on the labels - Malignant or Benign. For simplicity, we have given Malignant as “1” and Benign as “0”. In this project, we tried to understand the cancer detection process based on the given dataset. Our dataset includes many small pathology images to classify as labels - “1” or “0”. The project is implemented using Python. This project was a part of a Kaggle competition.

## Dataset Description
In this dataset, we are provided with many small pathology images to classify. Files are named with an image id. The trains_labels.csv file provides the ground truth for the images in the train folder. We are predicting the labels for the images in the test folder. A positive label indicates that the centre 32x32px region of a patch contains at least one pixel of tumour tissue. Tumour tissue in the outer region of the patch does not influence the label. This outer region is provided to enable fully convolutional models that do not use zero padding, to ensure consistent behaviour when applied to a whole-slide image. The original PCam dataset contains duplicate images due to its probabilistic sampling, however, the version presented on Kaggle does not contain duplicates. However, we have been provided with the same data and splits as the PCam benchmark.   

## The Algorithms used  
* Convolutional Neural Networks: A CNN is a Deep Learning algorithm which can take in an input image, assign importance (learnable weights and biases) to various aspects/objects in the image and be able to differentiate one from the other. We are using CNNs to classify metastatic tissues as malignant or benign (1 or 0). 
* Ensemble Learning: In this project, we took the prediction results from the various previous results and tried to combine up to three prediction files results using Ensemble Algorithm. We have used averaging and weighted averaging methods of ensemble learning.  

