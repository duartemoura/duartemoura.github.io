---
title: "Denoising Autoencoders"
excerpt: "Denoising FMNIST and MNIST datasets. <br/><img src='/images/dau.png' width='500' height='300'>"
collection: portfolio
---

In this project, I implement a denoising autoencoder using PyTorch to reconstruct clean images from noisy inputs. The model is trained on the MNIST and Fashion MNIST (FMNIST) datasets, each comprising 60,000 training images and 10,000 test images of handwritten digits and fashion items, respectively. Each image is 28x28 pixels in grayscale.

A denoising autoencoder is a neural network designed to remove noise from data by learning to map noisy inputs to their original, noise-free versions, effectively capturing a robust representation of the data. The architecture consists of two main components:

- **Encoder**: Compresses the input image into a lower-dimensional latent representation.
- **Decoder**: Reconstructs the original image from the latent representation.

The model is trained to minimize the mean squared error between the reconstructed and original images, enabling it to effectively denoise corrupted inputs.

<div style="text-align: center;">
  <img src="/images/dataset_FMNIST_model_Autoencoder3_var_0p01(1).png" alt="Denoising Autoencoder FMNIST Results" width="600">
  <p><em>Denoising Autoencoder applied to Fashion MNIST (FMNIST) dataset with noise variance of 0.01. The first row shows the original images, the second row shows noisy inputs, and the third row shows reconstructed outputs.</em></p>
</div>

<div style="text-align: center;">
  <img src="/images/dataset_MNIST_model_Autoencoder3_var_0p1(2).png" alt="Denoising Autoencoder MNIST Results" width="600">
  <p><em>Denoising Autoencoder applied to MNIST dataset with noise variance of 0.1. The first row shows the original images, the second row shows noisy inputs, and the third row shows reconstructed outputs.</em></p>
</div>


You can explore the project's code and detailed report here: [Denoising Autoencoder](https://github.com/duartemoura/denoising_autoencoder)