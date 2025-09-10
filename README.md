# Convolutional Autoencoder for Image Denoising

This repo contains two versions of a convolutional autoencoder designed for image denoising, applied to the MNIST dataset. The autoencoder removes noise from images to reconstruct clean versions. Below is an overview of the two versions included in this repository.

**Keyword**: Convolutional Autoencoder, MNIST, Denoise Images, Tensorflow, Sckit-image.

## Old version
- **Description**: This is the original implementation of the convolutional autoencoder, which was published in a scientific magazine. It includes the foundational architecture and methodology for denoising MNIST images.
    - Uses Mean Squared Error (MSE) as the loss function.
    - Optimized with the Adam optimizer.
- **File**: `CAE_DenoiseImage.ipynb`
This version was published in "Dong A University Journal of Science" in 2022
[DENOISING IMAGES USING CONVOLUTIONAL AUTOENCODER TECHNIQUE ](https://js.donga.edu.vn/index.php/daujs/article/view/9)

## New version (Improved Implemetation)
- Description: This is an updated and improved version of the convolutional autoencoder, addressing limitations of the old version and incorporating advancements in architecture and training methodology.
- Improvements: 
    - Enhanced Architecture: The autoencoder architecture has been refined with activation functions to better capture image features.
    - Different Loss Function: Use binary crossentropy instead of MSE.

## Repository Structure

- `CAE_Denoise_old_version`: The original published version of the autoencoder.
- `main.ipynb`: The improved version with enhanced architecture and loss function.
- `denoising_autoencoder.h5`: The saved model after improving.


## Requirements

- Python 3.9 or higher
- Libraries: `tensorflow`, `numpy`, `matplotlib`, `scikit-image`, `opencv-python`
- GPU support recommended for faster training (as implemented in the old version).

## Usage

1. **Old Version**:

   - Run `CAE_DenoiseImage.ipynb` in a Jupyter Notebook environment (preferably Google Colab with GPU support).
   - The notebook loads the MNIST dataset, trains the autoencoder, and generates denoised images.
   - Outputs include a training loss plot (`plot.png`) and sample reconstructions (`output.png`).

2. **New Version**:

   - Run `main.ipynb` to experiment with the improved autoencoder.
   - Note: The new version may require resolving NumPy compatibility issues (e.g., downgrading to `numpy<2` or updating dependent libraries like `ml_dtypes`).

## Future Work

- Further optimize the autoencoder architecture and explore advanced loss functions.
- Extend the model to handle more complex datasets and noise types.

