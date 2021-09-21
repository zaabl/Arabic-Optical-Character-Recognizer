# Arabic-Optical-Character-Recognizer
## Overview
This notebook builds an OCR for handwritten Arabic letters, research in OCR or optical character recognition started a long time ago in order to allow the computer to understand the words in any visual image, but the peak in OCR performances did happen in the deep learning era as it introduced advanced methods and techniques in order to achieve the OCR's outstanding outcomes and uses. 
The dataset used will be from Benha University, and the CNN will be build using Keras from TensorFlow.

## Dataset
The data-set is composed of 16,800 characters written by 60 participants, the age range is between 19 to 40 years, and 90% of participants are right-hand. Each participant wrote each character (from ’alef’ to ’yeh’) ten times on two forms as shown in Fig. 7(a) & 7(b). The forms were scanned at the resolution of 300 dpi. Each block is segmented automatically using Matlab 2016a to determining the coordinates for each block. The database is partitioned into two sets: a training set (13,440 characters to 480 images per class) and a test set (3,360 characters to 120 images per class). Writers of training set and test set are exclusive. Ordering of including writers to test set are randomized to make sure that writers of test set are not from a single institution (to ensure variability of the test set).

https://www.kaggle.com/mloey1/ahcd1
