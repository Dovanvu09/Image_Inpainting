
# Image Inpainting using Denoising Diffusion Probabilistic Models

## Overview

This project demonstrates the use of **Denoising Diffusion Probabilistic Models (DDPMs)** for **image inpainting**. Image inpainting is the process of filling in missing parts of an image, and DDPMs have shown to be effective in generating high-quality inpainted images by modeling the distribution of image data through a denoising diffusion process.

## Requirements

To run this notebook, you will need the following:

- Python 3.x
- Google Colab (for easy access to GPU resources)
- Necessary Python libraries:
  - TensorFlow
  - NumPy
  - OpenCV
  - Matplotlib
  - etc.

## Setup

1. **Mount Google Drive**: The notebook accesses files from your Google Drive. First, you will need to mount your Google Drive.

   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

2. **Navigate to the Working Directory**: Ensure you're in the correct directory where your files and models are stored.

   ```python
   %cd /content/drive/MyDrive/Diffusion-Models
   ```

## Steps for Inpainting

The notebook is organized into several sections that guide you through the image inpainting process:

1. **Loading and Preprocessing Data**: This section prepares the dataset for training and testing, including image preprocessing and splitting data.

2. **Model Architecture**: The Denoising Diffusion model architecture is defined here. This model performs iterative denoising steps to generate high-quality images.

3. **Training the Model**: In this section, the DDPM is trained on the image dataset. The training process involves learning the noise distribution and applying denoising steps to the images.

4. **Performing Inpainting**: Once the model is trained, this section demonstrates how to use the model to perform inpainting on an image by filling in missing parts with plausible content.

5. **Evaluation and Results**: The final section evaluates the model's inpainting performance and visualizes the inpainted images.

## How to Use

1. Clone the repository or download the notebook file.
2. Open the notebook in Google Colab or any local Jupyter environment.
3. Follow the instructions in the notebook to mount your Google Drive and navigate to the correct working directory.
4. Run the cells step by step to train the model and perform image inpainting.

## Results

After completing the inpainting process, the notebook will display the inpainted images alongside the original images for comparison. You can evaluate the quality of the inpainting and adjust the model parameters as needed.

## Acknowledgments

- **Denoising Diffusion Probabilistic Models**: Original research and implementations that inspired this notebook.
- **Google Colab**: Used for running the notebook and leveraging GPU resources for model training.

## License

This project is licensed under the MIT License.
