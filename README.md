# Visually-Perspective-Similarity-Metric-for-T2I-Models

This repository contains code to test different similarity metrics on Text-to-Image models

### Pre-trained models used

1. VGG16
2. CLIP (Contrastive Language-Image Pre-Training)

### Similarity metrics compared

1. Using $L^2$ Norm
$$\operatorname{sim}(v_1, v_2) = 1 - \|\hat{v_1} - \hat{v_2}\|_2$$
2. Cosine similarity
$$\operatorname{sim}(v_1, v_2) = \frac{v_1.v_2}{\|v_1\|\|v_2\|}$$

### Code
* `similarity_metric_test.ipynb`: generates the feature vectors of the images and the same images with gaussian or uniform noise using the VGG16 model and compares their $L^2$ Norm similarity scores.
* `stable_diffusion/stable_diffusion_similarity.ipynb`: generates images from stable diffusion model given same or different prompts and compares the $L^2$ Norm and cosine similarity scores.
* `dalle2/dalle_2.ipynb`: generates images from dalle2 model given same or different prompts.
* `dalle2/Dall_E2_similarity.ipynb`: compares the $L^2$ Norm and cosine similarity scores.
* `stable_diffusion/stable_diffusion_intermediate_results.ipynb`: generates each iteration of output images from stable diffusion model and compares the $L^2$ Norm and cosine similarity scores between each consecutive images.
