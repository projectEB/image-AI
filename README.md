# Image AI

A simple Python script to generate images from text prompts using the Stable Diffusion model.

## Description

This project provides a command-line interface to generate images based on user-provided text prompts. It uses the `diffusers` library from Hugging Face to run the Stable Diffusion v1.4 model.

## Getting Started

### Prerequisites

- Python 3.12 or later
- A Hugging Face account and an access token with permissions to use Stable Diffusion models.

### Installation

1.  Clone the repository:
    ```bash
    git clone <repository-url>
    cd Image-AI
    ```

2.  It is recommended to use a virtual environment:
    ```bash
    python -m venv .venv
    source .venv/bin/activate
    ```

3.  Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

### Usage
 
1.  Create a `.env` file by copying the template:
     ```bash
    python make_your_own_image_ai.py
    cp .env.template .env
     ```
2.  Open the `.env` file and add your Hugging Face token:
    ```
    HUGGING_FACE_TOKEN="your-token-goes-here"
    ```
3.  Run the script:
    ```bash
    python make_your_own_image_ai.py
    ```
4.  When prompted, enter a description of the image you want to create.
 
5.  The generated image will be displayed on your screen.

 ## Note
 The script will automatically detect and use the best available hardware for image generation (CUDA for NVIDIA GPUs, MPS for Apple Silicon, or CPU).