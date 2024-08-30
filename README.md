# Sketch to Real Image Conversion Using GANs

This repository contains the implementation of a Deep Convolutional GAN (DCGAN) for converting forensic sketches to realistic images. The project leverages the CUHK dataset to train the model, aiming to push the boundaries of AI in forensic science.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Project Overview

The primary goal of this project is to develop a machine learning model capable of converting hand-drawn forensic sketches into high-quality, lifelike images. This work has potential applications in forensic investigations where sketches are often used based on witness descriptions.

The model is built using a Deep Convolutional GAN (DCGAN) architecture, which consists of a generator and discriminator working together to produce realistic images from input sketches.

## Dataset

We are using the **CUHK Face Sketch Database (CUFS)**, which includes pairs of sketches and corresponding real images. This dataset is crucial for training the GAN model to accurately map sketch features to their realistic counterparts.

### Directory Structure

- **sketches/**: Contains all the sketch images.
- **photos/**: Contains all the corresponding real images.

**Dataset Paths:**
- Sketches: `/content/datasets/sketches`
- Photos: `/content/datasets/photos`

## Model Architecture

The model architecture consists of two primary components:

1. **Generator**: The generator takes input sketches and attempts to generate a realistic image. It is designed using convolutional and transpose convolutional layers to capture the fine details of the sketches.
  
2. **Discriminator**: The discriminator evaluates the generated images against the real images and helps the generator improve by providing feedback.

## Installation

To set up the project, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/sketch-to-real-image.git
   cd sketch-to-real-image

