# Project Name
Module 4 | Melanoma Detection Assignment


## General Information
Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

The objective is to build a CNN that can accurately detect the presence of Melanoma.

The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following diseases:
- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

Despite this being essentially a melanoma detector, the model is built from a multiclass perspective, such that it can accurately detect all 9 types of skin cancer presented above.

## Conclusions
A moderately deep CNN with 5 convolutional blocks and 3 dense hidden layers are used along with Dropouts, BatchNorm layers and a softmax output layer.

- In the initial stage the model overfitted significantly due to the lack of variation in the images.

- After introducing random variations, the training and validation accuracy (and loss) curves were growing closer together, which was promising. However, we could not conclude the presence or absence of overfitting due to the fact that now the model underfit the data. This meant that more training images were needed.

- We used the Augmentor package to fabricate augmented training images and used the augmented set to train the model. The results were much more promising.


## Contact
Created by [@somrikbanerjee] - feel free to contact me!