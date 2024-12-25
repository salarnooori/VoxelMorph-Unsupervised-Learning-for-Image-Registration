# VoxelMorph: Unsupervised Learning for Image Registration

This repository contains the implementation of the VoxelMorph framework for image registration using deep learning. The method leverages a convolutional neural network to predict a deformation field that aligns a moving image to a fixed image. The training process minimizes a loss function that combines similarity and smoothness terms.

## Proposed Method
VoxelMorph uses unsupervised learning to register images by minimizing a loss function reflecting spatial correspondence. The model consists of:
- **Encoder-Decoder Network**: Extracts features from input images and generates the deformation field.
- **Flow Field**: Represents pixel displacements for image alignment.

## Dataloader
The dataloader prepares image pairs for training and evaluation.

## Loss Function
The total loss is a weighted sum of similarity and smoothness losses:
- **Similarity Loss**: MSE and cross-correlation to match pixel intensities.
- **Smoothness Loss**: Regularizes the deformation field to encourage smooth transformations.

$$
L_{\text{total}} = L_{\text{similarity}} + \lambda \cdot L_{\text{smooth}}
$$

## Training
Train the model using the defined loss functions and plot the results.

## Results
Visualize the alignment of moving and fixed images after registration.

## References
- [VoxelMorph Paper](https://arxiv.org/pdf/1809.05231)

## Contributors
Feel free to open issues or pull requests.

## License
MIT License
