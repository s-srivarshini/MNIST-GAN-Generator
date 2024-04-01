# MNIST-GAN-Generator
This project contains Python code for training a Generative Adversarial Network (GAN) that learns to generate images resembling handwritten digits from the MNIST dataset. It includes both the Generator and Discriminator models, training loops, and utility functions for visualizing the generated images and training loss over time.

## Getting Started
### Installation
To run the notebook and replicate the findings, ensure you have the following Python packages installed:

```bash
pip install torch
pip install torchvision
pip install matplotlib
pip install tqdm
```
### Models
**Generator**: Takes a noise vector as input and generates images of dimensions 28x28, resembling MNIST digits.

**Discriminator**: Takes an image as input and outputs a probability indicating whether the image is real or generated.

### Training Process
The training process involves alternating between training the discriminator and the generator. The discriminator is trained first by feeding it real and generated images, followed by training the generator to fool the discriminator.

### Visualizations
- Generated images are periodically saved to visually assess the quality of generated digits.
- A plot of discriminator and generator losses over training batches is saved to analyze the training process.
