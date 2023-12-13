
# Crop Type Segmentation with Swin Unet:  To account for crops phenology, time series images are averaged.

## Overview

This repository contains code for a Crop Type Segmentation model based on the Swin Transformer architecture (attention approach). The model is trained to segment different crop types from satellite imagery. The data loading mechanisms considered the average of time series images for each satellite. 


## 1. Data Source

The dataset used for training and validation is sourced from Google Cloud Platform (GCP). The dataset includes images from  three satellites namely Planet, sentinel-1 and Sentinel-2.

### .2. Accessing Data on GCP

To access the dataset on GCP, follow these steps:

1. **GCP Account Setup:**
   - Ensure you have access to the Google Cloud Platform with the necessary permissions.

### Clone Repository

Use the following command to clone the repository:

`https://github.com/IntroToDeepLearning-2023/swin_unet_dates_averaged`
     
2. **Dataset Location:**
   - The dataset is stored in a GCP Storage Bucket. You can find the dataset at the following location: `gs://data_ctm/data/data/africa_crop_type_mapping/ghana/`.
     
3. **Downloading the Dataset:**
   - Use the following command to list files in the dataset folder:

     ```bash
     !gsutil ls gs://data_ctm/data/data/africa_crop_type_mapping/ghana/
     ```

     You can download specific files using `gsutil cp` command.

     ```bash
     !gsutil cp gs://data_ctm/data/data/africa_crop_type_mapping/ghana/*/your_file.
     ```
4. **Data Loading:**
   - The training and validation scripts in this repository are configured to load data directly from the GCP Storage Bucket. Ensure that your GCP credentials are set up correctly on the machine running the code.

## 3. Model Architecture

The segmentation model is based on the Swin Transformer architecture (Extended to Swin-Unet), a recent advancement in computer vision. The model is designed for effective segmentation of crop types from satellite imagery.

## 4. Running Jupyter Notebook

1. **Training:**

The Jupyter notebook (`IDL_Swin_TA.ipynb`) includes the complete pipeline for training the model. Make sure to run the notebook from the to set up the necessary dependencies and configurations.

2. **Configuration:**

Adjust the training configurations in the `config` dictionary in the Jupyter notebook. Key configurations include the number of epochs, learning rate, loss weights, etc.

3. **Evaluation:**

The evaluation is also done in (`IDL_Swin__TA.ipynb`) designed to assess the performance of the trained model on a separate validation dataset.

4. **Results:**

The performance of the trained model are printed at the end of the notebook in terms of accuracy and other relevant metrics.

Important Note:

This is a general overview of the visualization process.

## Contributors

- **Deo Uwimpuhwe**
  - Program: MSECE 2024
  - Email: [duwimpuh@andrew.cmu.edu](mailto:duwimpuh@andrew.cmu.edu)

- **Gustave Bwirayesu**
  - Program: MSECE 2024
  - Email: [gbwiraye@andrew.cmu.edu](mailto:gbwiraye@andrew.cmu.edu)

- **Eric Maniraguha**
  - Program: MSIT 2024
  - Email: [emanirag@andrew.cmu.edu](mailto:emanirag@andrew.cmu.edu)

- **Bienvenue Jules Himbaza**
  - Program: MSECE 2024
  - Email: [hjulesbi@andrew.cmu.edu](mailto:hjulesbi@andrew.cmu.edu)

