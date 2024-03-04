# Generative Adversarial Networks (GANs) Project: GenAI

Welcome to the GenAI project! This repository contains a PyTorch implementation of a basic Generative Adversarial Network (GAN) designed to generate images that resemble handwritten digits from the MNIST dataset. Our GAN model consists of two main components: a Generator and a Discriminator, working against each other to produce highly realistic images.

## Project Overview

The GenAI project leverages the power of GANs to understand and generate digit images that mimic the style of the MNIST dataset. This is accomplished through the adversarial process between two networks:

- **Generator (Gen)**: Learns to generate plausible digit images.
- **Discriminator (Disc)**: Learns to distinguish between real images from the MNIST dataset and fake images produced by the Generator.

As the training progresses, both networks improve their capabilities, with the Generator producing increasingly realistic images and the Discriminator becoming better at identifying real images from the fake ones.

## Libraries and Tools Used

- `torch`: The core PyTorch library providing tensor computation and deep learning functionalities.
- `torch.nn`: A sub-library of PyTorch to build neural networks.
- `torch.optim`: Provides optimization algorithms for neural networks.
- `torchvision`: Offers datasets, model architectures, and image transformations for computer vision.
- `matplotlib`: A plotting library for creating static, interactive, and animated visualizations in Python.
- `tqdm`: A library for displaying progress bars during loops.

## Key Functions and Classes

- `genBlock(inp, out)`: Defines a block for the Generator model.
- `Generator`: The neural network model for generating images.
- `discBlock(inp, out)`: Defines a block for the Discriminator model.
- `Discriminator`: The neural network model for discriminating between real and fake images.
- `show(tensor, ch, size, num)`: Utility function to visualize the images generated by the GAN.
- `calc_gen_loss`: Calculates the loss for the Generator.
- `calc_disc_loss`: Calculates the loss for the Discriminator.

## Getting Started

To get started with the GenAI project, clone this repository and install the necessary dependencies listed above. You can then run the provided Jupyter notebook or Python script to train the GAN models on your machine.

Ensure you have PyTorch and torchvision installed, along with matplotlib for visualization.

```bash
git clone https://github.com/Harshverdhan19/GenAI.git
cd genai
# Activate your virtual environment or conda environment
pip install torch torchvision matplotlib tqdm
# Run the script or notebook
