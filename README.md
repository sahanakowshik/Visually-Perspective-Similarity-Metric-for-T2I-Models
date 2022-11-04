# Visually-Perspective-Similarity-Metric-for-T2I-Models

This repository contains code to test different similarity metrics on Text-to-Image models

### Pre-trained models used

1. VGG16
2. CLIP (Contrastive Language-Image Pre-Training)

### Similarity metrics compared

1. Using L2 Norm
$$similarity(v_1, v_2) = 1 - \|\hat{v_1} - \hat{v_2}\|_2$$
2. Cosine similarity
$$similarity(v_1, v_2) = \frac{v_1.v_2}{\|v_1\|\|v_2\|}$$

### Code

The file `similarity_metric_test.ipynb` generates the feature vectors of the images and the same images with gaussian or uniform noise using the VGG16 model and compares their L2 Norm similarity scores.
The file `stable_diffusion.ipynb` generates images from stable diffusion model given same or different prompts and compares the L2 Norm and cosine similarity scores.
