# Crop Type Segmentation with Swin Unet Transformer 🛰️

This repository contains the code for training a crop type segmentation model using the Swin Transformer architecture. The model is designed for segmentation tasks on remote sensing data, specifically for classifying different crop types in satellite imagery.
...

## 1. Table of Contents

- [Overview](#overview)
- [Requirements](#requirements)
- [Dataset](#dataset)
- [Usage](#usage)
- [Training](#training)
- [Results](#results)
- [License](#license)

## 2. Overview

The project uses the Swin Transformer architecture for crop type segmentation. The model is implemented using PyTorch and trained using a custom dataset. The training script logs metrics and results to WandB for easy tracking and visualization.

## 3. Requirements

- Python 3.6 or later
- PyTorch
- WandB
- Other dependencies (specified in `requirements.txt`)

Install dependencies:

```bash
pip install -r requirements.txt`
```

## 4. Dataset

The dataset used for training is the SustainBenchDataset, and it is loaded using the CropTypeMappingDataset class. Ensure you have the dataset available or replace it with your custom dataset.

## 5. Usage

Clone the repository:

`https://github.com/IntroToDeepLearning-2023/swin_unet_dates_averaged`
`cd crop-type-segmentation`

Install dependencies:

`pip install -r requirements.txt`

1. Set up your WandB account and obtain an API key. Update the API key in the training script.

2. Configure your training parameters in the script.

## 6. Training

Run the training script:

`python train.py`
The script logs metrics, loss, and accuracy to WandB for easy monitoring.

## 7. Results

The trained model and evaluation results can be found in the models/ directory. The best-performing model is saved as best.pth. You can load this model for inference or continue training.

Important Note:

This is a general overview of the visualization process.

## 8. Contributors

- **Deo Uwimpuhwe**
  - Program: MECE 2024
  - Email: [duwimpuh@andrew.cmu.edu](mailto:duwimpuh@andrew.cmu.edu)

- **Gustave Bwirayesu**
  - Program: MECE 2024
  - Email: [gbwiraye@andrew.cmu.edu](mailto:gbwiraye@andrew.cmu.edu)

- **Eric Maniraguha**
  - Program: MSIT 2024
  - Email: [emanirag@andrew.cmu.edu](mailto:emanirag@andrew.cmu.edu)

- **Bienvenue Jules Himbaza**
  - Program: MECE 2024
  - Email: [hjulesbi@andrew.cmu.edu](mailto:hjulesbi@andrew.cmu.edu)

# Happy Code 😄

> "Attention is not just the key to understanding, it's the magic ingredient in the deep learning recipe." - Anonymous Deep Learning Enthusiast

Remember, in the world of deep learning, even the errors are "feature not bugs" – they're just misunderstood neurons doing their best to impress the model! 😄🤖


