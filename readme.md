Introduction

This repository contains all the necessary files that are needed to reproduce the results as described in the paper *Skin_Cancer_Capstone_Sept28.pdf* 

There are 5 directories and 6 Juypter notebooks. A brief description for each one these items are provided below:

**cifar** - directory for cifar-10 images in PNG format

**CLR** - directory contains the cyclic learning rate code with proper licensing term and condition

**Training_Data_Sq_orig_added_images** - directory contains 5,000 images altogether from oversampling original 2,000 images, augmented images have been rotated randomly

**Test_Data_Sq_orig** - original 2017 ISIC 600 test data that have been cropped and resized to 300x300 pixels

**Validation_Data_Sq_orig** - original 2017 ISIC 150 validation data that have been cropped and resized to 300x300 pixels

**ISIC_features-All-in-One.ipynb** -  extract features from training images for bottleneck training

**top_model_base-ISIC-AUC-All-in-One-plots-CV.ipynb**  - conduct 5-folds CV for the top layer

**top_model_base-ISIC-AUC-All-in-One-stacking-different_models.ipynb**  - train a stacked ensemble for the top layer

**fine_tune-CLR-benchmark-with-VGG_and_ResNet50-CIFAR10.ipynb** - fine tuning for the CIFAR-10 dataset

**fine_tune-CLR-ISIC-with-VGG_Layer_1.ipynb**  - VGG16 fine tuning for the 2017 ISIC cancer dataset

To extract features and train top models, one can follow these steps:

1. set parameters in **ISIC_features-All-in-One.ipynb** then run the program
2. it should generate multiple output files, depending on how many models are chosen
3. run either **top_model_base-ISIC-AUC-All-in-One-plots-CV.ipynb** or **top_model_base-ISIC-AUC-All-in-One-stacking-different_models.ipynb**

For fine tuning:

1. set parameters in the notebook **fine_tune-CLR-ISIC-with-VGG_Layer_1.ipynb**
2. run the notebook, it will read image files directly from different directories and output results interactively


