# Waifu-Generator


So this repo contains a Notebook I made last year, in an attempt to generate Waifus (female anime character) faces using AutoEncoders. Although I created the repo for this project, I never really felt like throwing this project up on GitHub till now 😅

Anyways, feel free to check the notebook out for some fun ML stuff. The model took a couple of hours to train, and I used Kaggle's kernels for it. Dataset source can be found [here](https://www.kaggle.com/splcher/animefacedataset), and my Kaggle Kernel [here](https://www.kaggle.com/naimish123/waifugenerator-ae)

All images were resized to 32x32, and the latent vector exists in 256 dimensions. I originally wanted to train it on 80x80 images, but due to memory issues and lack of access to a GPU, I settled for this resolution. I'll probably visit this project again in the future, if time and compute resources permit, to train a higher resolution, deeper AutoEncoder. Or even a GAN, who knows 😄

---

# Reconstruction results

![Reconstructed Images](https://github.com/Naimish240/waifu-generator/blob/master/images/WG_reconstructions.png)

---

# Generated Images

![Generated Images](https://github.com/Naimish240/waifu-generator/blob/master/images/WG_generated_images.png)

---

# Latent Space

![Latent Space](https://github.com/Naimish240/waifu-generator/blob/master/images/WG_latentSpace.png)
