# Project Name
> The project uses a multiclass classification model using Custom convolutional neural network in Tensor flow to accurately detect Melanoma


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. 
- In this assignment we create a solution/model that can evaluate images and help alert dermatologists about the presence of melanoma thus reducing a lot of manual effort needed in diagnosis.
- The source/input dataset consists of 2357 images of 9 malignant and benign oncological disease classes, which were formed from the International Skin Imaging Collaboration (ISIC)
- The model uses data augmentation techniques to resolve the underfitting/overfitting issues and rectify class imbalances.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- The first iteration of the model without using drop out tend to overfit.
- The Training accuracy dropped significantly after using the drop out and data augmentation (from 93% to 55%) in model-2. However the Test accuracy dropped marginally from (58% to 51%). 
- Since, train accuracy is low it seemed to indicate undefitting. We thus had to augment our intial dataset with additional images using augmentor
- We tried to re-balance the category class imbalance by increasing the number of images per class category (Augmentation) proportionately. This resulted in better training and test accuracy.
- By previously applying data augmentation we also improved the data quality by adding rotated, flipped and zoomed versions of the source images.
- We also added additional drop out layers in subsequent models that helped reduce the model complexity and generalise the model further.
- We can conclude that the resultant model is now more generalised and is not overfitting.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Panda
- Numpy
- seaborn
- matplotlib
- tensorflow
- keras
- pathlib
- glob
- augmentor

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by Kaggle
- This project was based on courses taken from upgrad.


## Contact
Created by [@abe-twistedtech] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->