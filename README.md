# Arabic-Optical-Character-Recognizer
## Overview
This notebook builds an OCR for handwritten Arabic letters, research in OCR or optical character recognition started a long time ago in order to allow the computer to understand the words in any visual image, but the peak in OCR performances did happen in the deep learning era as it introduced advanced methods and techniques in order to achieve the OCR's outstanding outcomes and uses. 
The dataset used will be from Benha University, and the CNN will be build using Keras from TensorFlow.

## Dataset
The data-set is composed of 16,800 characters written by 60 participants, the age range is between 19 to 40 years, and 90% of participants are right-hand. Each participant wrote each character (from ’alef’ to ’yeh’) ten times on two forms as shown in Fig. 7(a) & 7(b). The forms were scanned at the resolution of 300 dpi. Each block is segmented automatically using Matlab 2016a to determining the coordinates for each block. The database is partitioned into two sets: a training set (13,440 characters to 480 images per class) and a test set (3,360 characters to 120 images per class). Writers of training set and test set are exclusive. Ordering of including writers to test set are randomized to make sure that writers of test set are not from a single institution (to ensure variability of the test set).

https://www.kaggle.com/mloey1/ahcd1

## Model's Architecture
We will use keras for the creation of our model, we will start by creating a function for use to create our model, we will set the activation, optimizer and our initializing method as variables for us to easly modifiy it in the hyper-parameter tuning phase.We will start by creating our first convolutional layer and setting up the input shape, we will create additional pooling layer along with a batch normalization layer, then we will add three convolutional layers with the same structure but the the double size of filters each layer.Then we will flatten our layer preparing it for the fully connected layers, we will use a small neurons numbered layer with a drop out layer, batch normalization and we will add an L2 regularizer so we will control the overfitting.


![architecture](https://user-images.githubusercontent.com/32912214/134214756-0a8df267-067e-4247-943a-b83606670960.png)

## Acknowledgments

• Author: **Hossam Zaabl**

https://github.com/zaabl

• A. El-Sawy, M. Loey, and H. EL-Bakry, “Arabic handwritten characters recognition using convolutional neural network,” WSEAS Transactions on Computer Research, vol. 5, pp. 11–19, 2017.

https://doi.org/10.1007/978-3-319-48308-5_54

https://link.springer.com/chapter/10.1007/978-3-319-48308-5_54

• A. El-Sawy, H. EL-Bakry, and M. Loey, “CNN for handwritten arabic digits recognition based on lenet-5,” in Proceedings of the International Conference on Advanced Intelligent Systems and Informatics 2016, vol. 533, pp. 566–575, Springer International Publishing, 2016.

https://www.wseas.org/multimedia/journals/computerresearch/2017/a045818-075.php

• Loey, Mohamed, Ahmed El-Sawy, and Hazem El-Bakry. "Deep learning autoencoder approach for handwritten arabic digits recognition." arXiv preprint arXiv:1706.06720 (2017).
https://arxiv.org/abs/1706.06720

• Amr Hendy, Arabic Handwritten Image Recognition

https://github.com/AmrHendy/Arabic-Handwritten-Images-Recognition
