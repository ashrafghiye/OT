# Optimal Transport in Generative Adversarial Networks

<p align="center">
  <img src="https://user-images.githubusercontent.com/24767888/116453334-0ab62200-a85f-11eb-8fca-1a040d366664.png" />
</p>


This project explores Optimal Transport variants in Generative Adversarial Network.
The goal is to implement recent GANs with enhanced loss function that builds on Optimal Transport Theory.

## Context

[Optimal Transport](https://marcocuturi.net/ot.html) course taught at ENSAE with prof. [Marco CUTURI](https://marcocuturi.net/).

## Motivation

Despite their success in the previous years, Generative Adversarial Network suffers from major problems such as training instability and mode collapse. Most of these problems are related to the choice of the BCE loss which is related to Jensen-Shannon divergence. This loss does not take into account the topological space of probability distributions.

In short, **Optimal Transport can be characterized as the natural geometry to compare probability distributions**. Thus using ideas from OT, we can define new loss functions that induce better geometric properties for our learning process. 

We will discover two flavours of OT in Generative Models and Statistical Learning in general: **Using a regularized version of the original OT problem [Cuturi' 13] we can define the Sinkhorn divergence between two measures, and using the dual formation of optimal transport we can use neural network to approximate 1-Wasserstein distance between two densities.**

## Content

- Jupyter notebook `OT-GANs.ipynb` which is a step by step guide of the study on Sinkhorn divergence and OT-GANs.

- Jupyter notebook `W-GANs.ipynb` which is a step by step guide of the study on Wasserstein distance and Wasserstein-GANs.

- The resulted plots are saved in `images`.

- The final report with detailed analysis is not included yet.

## References

[1](https://arxiv.org/abs/1706.00292) Aude Genevay, Gabriel Peyré, Marco Cuturi: **Learning Generative Models with Sinkhorn Divergences**

[2](https://arxiv.org/abs/1803.05573) Tim Salimans, Han Zhang, Alec Radford, Dimitris Metaxas: **Improving GANs Using Optimal Transport**

[3](https://arxiv.org/abs/1701.07875) Martin Arjovsky, Soumith Chintala, Léon Bottou: **Wasserstein GAN**

[4](https://arxiv.org/abs/1704.00028) Ishaan Gulrajani, Faruk Ahmed, Martin Arjovsky, Vincent Dumoulin, Aaron Courville: **Improved Training of Wasserstein GANs**

