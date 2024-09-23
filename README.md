# U-Net for Polyp Segmentation

This repository contains the implementation of a U-Net model for the segmentation of polyps from gastrointestinal tract images using the Kvasir-SEG dataset. The project aims to automate the detection and delineation of polyps to improve the efficiency and effectiveness of colorectal cancer screening.

## Dataset

The dataset used in this project is the [Kvasir-SEG dataset](https://datasets.simula.no/kvasir/), which contains gastrointestinal tract images with corresponding segmentation masks for polyps. Make sure to download the dataset and place it in the appropriate directory.

## Model Architecture

The model architecture is based on the U-Net architecture, which is widely used for image segmentation tasks.

### Key Components

- **Input Layer**: Accepts images of size 256x256 pixels with three color channels.
- **Convolutional Layers**: Multiple convolutional layers with ReLU activation and He initialization.
- **MaxPooling**: Reduces the spatial dimensions of the feature maps.
- **Transposed Convolution**: Upsamples the feature maps in the expansive path.
- **Concatenation**: Merges feature maps from the encoder with those from the decoder.

## Results

The model achieves an accuracy of approximately 98% on the validation set. Key metrics include:

- **True Positives (TP)**: 748415
- **False Positives (FP)**: 222050
- **False Negatives (FN)**: 317993
- **Recall**: 0.701
- **Precision**: 0.771
- **F1 Score**: 0.735

## Usage

## Acknowledgements

- [Kvasir-SEG Dataset](https://datasets.simula.no/kvasir/)
- [U-Net Paper](https://arxiv.org/abs/1505.04597)
