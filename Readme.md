# Real Time Semantic Segmentation using Efficient Neural Network

## Project Overview

Semantic segmentation is a computer vision task where every pixel in an image is classified into a specific category. This project implements ENet, a lightweight deep neural network optimized for real-time segmentation with low latency. The model is tested on the CamVid dataset, and has achieved efficient segmentation performance at 10 FPS with a pixel accuracy of 75%.

## Languages & Tech stack

- **Python** for implementation.
- **PyTorch** for Deep Learning framework.
- **CamVid** for dataset.


## Methodology

- **Model Architecture**
    - ENet uses an encoder-decoder structure, optimized for speed and efficiency.
    - Early downsampling and dilated convolutions help reduce the number of computations.

- **Implementation**
    - The model is trained using 367 training images, validated on 101 images, and tested on 233 images.
    - Hyperparameter tuning: Learning rate (5×10⁻⁴), batch size (5), weight decay (2×10⁻⁴).

- **Training & Testing**
    - The model is trained for 100 epochs, and the loss converged effectively.
    - The segmentation masks were evaluated using Pixel Accuracy, IoU, and F1 Score.


## Results

- Per-pixel accuracy - 75%.
- IoU - 0.51.
- F1 score - 0.64.
