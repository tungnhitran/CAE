# Convolutional Autoencoder for Image Denoising

This repo contains two versions of a convolutional autoencoder designed for image denoising, applied to the MNIST dataset. The autoencoder removes noise from images to reconstruct clean versions. Below is an overview of the two versions included in this repository.
## Old version
- File: 'CAE_DenoiseImage.ipynb'
- Trained on grayscale MNIST images.
- Description: This is the original implementation of the convolutional autoencoder, which was published in a scientific magazine. It includes the foundational architecture and methodology for denoising MNIST images.
- Uses Mean Squared Error (MSE) as the loss function.
- Optimized with the Adam optimizer.
- Includes basic data augmentation techniques.