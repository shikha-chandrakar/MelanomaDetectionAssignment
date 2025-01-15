# Melanoma Detection Assignment
> Problem statement: To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.
The data set contains the following diseases:

Actinic keratosis
Basal cell carcinoma
Dermatofibroma
Melanoma
Nevus
Pigmented benign keratosis
Seborrheic keratosis
Squamous cell carcinoma
Vascular lesion


## Conclusions
 Class Rebalancing:
- Helped reduce overfitting, as evidenced by a decrease in loss.
- However, it led to a significant drop in accuracy.
  
 Initial Training Without Augmentation:
- Training the model without using an ImageDataGenerator resulted in severe overfitting.
- The model performed well on the training data but failed to generalize effectively on validation data.
  
Introduction of Dropout and ImageDataGenerator:
- Dropout layers were added to reduce overfitting by preventing reliance on specific neurons.
- The ImageDataGenerator augmented the training data, improving diversity and reducing overfitting.
  
Incorporating Batch Normalization and Augmentation:
- Batch normalization stabilized the training process and improved convergence.
- Data augmentation further enhanced the model’s robustness by creating more varied training samples.
  
Overall Impact:
- These steps collectively improved the model’s ability to generalize and reduced overfitting.


## Technologies Used
- jupyter notebook - 7.0.8
- matplotlib library
- Keras
- pandas - Pandas version: 2.2.2

## Acknowledgements
- This project was done as part of UpgradC66 Batch - ML/AI project under CNN module.
