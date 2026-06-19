# Conditional GANs (cGAN)

## What is a Conditional GAN?

A standard GAN generates random outputs from noise — you have no control over what comes out. A **Conditional GAN (cGAN)** fixes this by feeding an extra label/condition `y` into both networks:

- **Generator:** `G(z, y) → image` — noise `z` + condition `y` (e.g. a class label)
- **Discriminator:** `D(x, y) → real/fake` — judges whether image `x` is real *given* condition `y`

This lets you direct generation — e.g. "generate a face with blue eyes" instead of getting whatever the model feels like producing.

---

## 📚 Papers

- **Conditional Generative Adversarial Nets** — Mirza & Osindero, 2014. [arXiv:1411.1784](https://arxiv.org/abs/1411.1784) — the original cGAN paper.
- **Unsupervised Representation Learning with Deep Convolutional GANs (DCGAN)** — Radford et al., 2015. [arXiv:1511.06434](https://arxiv.org/abs/1511.06434) — the convolutional architecture most cGANs are built on.

## 🎥 Videos

- **[Aladdin Persson — PyTorch Conditional GAN from Scratch](https://www.youtube.com/watch?v=Snqb7Usrauw)** — full PyTorch implementation walkthrough.
- **[DeepLearning.AI — GANs Specialization](https://www.deeplearning.ai/courses/generative-adversarial-networks-gans-specialization/)** — Course 1 covers building GANs, DCGANs, and conditional GANs step by step.
