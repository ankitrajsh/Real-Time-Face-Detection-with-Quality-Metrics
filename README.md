# Webcam Face Detection and Quality Analysis

This repository provides a solution for capturing images from a webcam, analyzing their quality, and detecting faces using advanced techniques. It is designed to ensure that only high-quality images are processed and saved.

## Features

- **Webcam Integration**: Capture images directly from your webcam using JavaScript within a Colab notebook.
- **Face Detection**: Detect faces in the captured images using the RetinaFace library.
- **Image Quality Analysis**: Evaluate images based on:
  - **Brightness**: Measures average brightness.
  - **Contrast**: Computes contrast using standard deviation.
  - **Noise**: Estimates noise level by variance.
  - **Sharpness**: Assesses sharpness using Laplacian variance.
- **Quality Thresholds**: Apply predefined thresholds for image quality attributes to filter out low-quality images.
- **Bounding Box Drawing**: Draw rectangles around detected faces and save the processed image if it meets the quality criteria.
- **Error Handling**: Gracefully handle issues with webcam access or image processing.

## Installation

To use this repository, you will need to set up a Colab notebook with the following dependencies:
- OpenCV
- NumPy
- PIL
- RetinaFace
- IPython
- Google Colab

You can install the necessary Python libraries using pip:

```bash
pip install opencv-python-headless numpy pillow retinaface ipython google-colab
