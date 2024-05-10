# Diffusion Model with U-Net for Road Sign Generation

This project implements a generative diffusion model using a U-Net architecture to generate road signs. The dataset used contains 33,000 images of road signs at a resolution of 32x32 pixels. This is university project
for neural network course.

## Project Overview

### Problem Statement
- **Task**: Generative modeling of road signs.
- **Dataset**: Contains 33,000 images of road signs at a resolution of 32x32 pixels.

### Solution
- **Model Architecture**: A U-Net-based generative diffusion model designed specifically for image generation.
- **Key Features**:
  - Implementation of a denoising diffusion probabilistic model.
  - U-Net architecture for improved performance.
  - Support for conditional and unconditional generation.

### Model Components
1. **U-Net Architecture**:
   - Encoder-decoder architecture with skip connections.
   - Residual blocks for efficient feature learning.

2. **Diffusion Model**:
   - Forward process to add noise.
   - Reverse process to remove noise using U-Net (learing goal: predicting orginal image).

### Training and Generation Pipeline
1. **Training Process**:
   - Train the U-Net model using a forward and reverse diffusion process.
   - Use the denoising score matching objective to minimize reconstruction loss.

2. **Generation Process**:
   - Generate road sign images from random noise using the reverse diffusion process.
