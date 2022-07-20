## Accurately detect melanoma using CNN

> To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. 
It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of 
melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

> The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.


> The data set contains the following diseases:

- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion


## Table of Contents
* [General Info](#general-information)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)

## General Information
- To detect Skin cancer accurately using images by developing CNN Model
- Skin Cancer dataset is being used
- Defining a 2 layered CNN model to train the image dataset.
- Doesn't leverage Transfer learning techniques

## Conclusions
- Model 0: Started with 2 layer CNN model. Model is overfit. (Training accuracy: 90% , Validation accuracy: 58%)
- Model 1 with dropout: Added few dropout layers then the model is underfit. (Training accuracy: 60% , Validation accuracy: 56%)
- Model 2: Added few more convolutional layers to the base model. Metrics are not improved.(Training accuracy: 56% , Validation accuracy: 55%)
- Model 3: Introduced data augumentation layer in the model with few options like rotation and flip.(Training accuracy: 58% , Validation accuracy: 57%). Model is underfir
- Model 4 with Augumentation: Did augumentation with augumentor to deal with class imbalance problem. (Training accuracy: 90% , Validation accuracy: 82%)
- Accuracy can still be improved by training the model for more epochs using the same CNN model
- Accuracy can also be improved by using more CNN and or Dense layers in the model.

## Technologies Used
- Keras
