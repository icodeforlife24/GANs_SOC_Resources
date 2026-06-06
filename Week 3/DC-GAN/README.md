## DC-GAN

DC-GAN (Deep Convolutional Generative Adversarial Network) is a GAN architecture that uses convolutional layers in both the generator and discriminator to generate realistic images.

### Overview
- The **generator** creates images from random noise.
- The **discriminator** distinguishes real images from fake ones.
- Both networks are trained adversarially, improving each other over time.

### Main advantages
- Better image quality than basic GANs
- Learns spatial features effectively using CNNs
- More stable training with common design choices like batch normalization

### Typical components
- Strided convolutions
- Batch normalization
- ReLU in the generator
- Leaky ReLU in the discriminator

### Applications
- Image synthesis
- Data augmentation
- Research in generative modeling

### Resources
-[Video Tutorial](https://youtu.be/-8S1KL7yod0?si=Oj7p6CWL-Jk0kH-G)
-[Tutorial](https://www.geeksforgeeks.org/machine-learning/deep-convolutional-gan-with-keras/)
-[Research Paper](https://arxiv.org/abs/1511.06434)