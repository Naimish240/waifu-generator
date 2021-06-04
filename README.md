# Waifu-Generator


So this repo contains a Notebook I made last year (Sept 2020), in an attempt to generate Waifus (female anime character) faces using AutoEncoders. Although I created a repo for this project, I never really felt like adding this project to my GitHub profile till now 😅

Anyways, feel free to check the notebook out for some fun ML stuff. The model took a couple of hours to train, and I used Kaggle's kernels for it. Dataset source can be found [here](https://www.kaggle.com/splcher/animefacedataset), and my Kaggle Kernel [here](https://www.kaggle.com/naimish123/waifugenerator-ae)

All images were resized to 32x32x3, and the latent vector exists in 256 dimensions. I originally wanted to train it on 80x80x3 images, but due to memory issues and lack of access to a GPU, I settled for this resolution. I'll probably visit this project again in the future, if time and compute resources permit, to train a higher resolution, deeper AutoEncoder. Or even a GAN, who knows 😄

One thing to note about AutoEncoders, is that the outputs they give tend to be a bit blurry. This is mainly attributed to using MSE as a loss function. GANs were invented primarily to address this issue, and the discriminator does a very good job (compared to an autoencoder, atleast) at generating images without too many artifacts.

The AutoEncoder was trained for only 150 epochs, and had a small latent dimension of 256. Increasing the latent vector size and increasing the number of epochs have been proven to generate better results in other similar projects, and the same probably holds true here.

There were 3 mains steps involved in this project:
1. Training an AutoEncoder to Reconstruct the images.
2. Generating images by randomly sampling from the Latent Space.
3. Visualising the Latent Space through t-SNE.

The results of each of the steps can be found below:

---

# 1. Reconstruction results

![Reconstructed Images](https://github.com/Naimish240/waifu-generator/blob/master/images/WG_reconstructions.png)

---

# 2. Generated Images

![Generated Images](https://github.com/Naimish240/waifu-generator/blob/master/images/WG_generated_images.png)

---

# 3. Latent Space

![Latent Space](https://github.com/Naimish240/waifu-generator/blob/master/images/WG_latentSpace.png)
