# Variational Autoencoder on CelebA

This project implements a convolutional **Variational Autoencoder (VAE)** trained on the CelebA dataset.  
The goal is to learn a latent representation of faces and explore how different latent dimensions control interpretable attributes such as **smiling, eye openness, and hairstyle**.

---

## Features
- Convolutional VAE with encoder/decoder symmetry
- Training with KL annealing and configurable reconstruction loss (BCE or MSE)
- Reconstruction of input images
- Random sampling from the latent space
- Latent traversals to visualize how attributes change when varying individual latent dimensions
- Scripts for correlating latent variables with CelebA attribute labels

---

## Latent Attribute Manipulation
We identified latent dimensions that influence:
- **Smile**  
- **Eye Openness**  
- **Hairstyle**  

By varying only those dimensions and keeping others fixed, we generated smooth transitions in the output images.

Example traversal (smile attribute):

![Smile Traversal](vae_out/smile_traversal.png)

---

## How to Run
1. Clone this repo:
   ```bash
   git clone https://github.com/yourusername/vae-celeba.git
   cd vae-celeba
