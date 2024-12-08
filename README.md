# fine-tune-stable-diffusion-on-Cartoon-dataset

This project fine-tunes the Stable Diffusion model using Hugging Face's Diffusers library on a cartoon dataset. The fine-tuned model generates custom cartoon characters from text prompts.

## Features
- Fine-tuning Stable Diffusion with LoRA (Low-Rank Adaptation)
- Training on the **Rick and Morty captions dataset**
- Generating high-quality cartoon images
- Integration with WandB for experiment tracking
- Model hosting on Hugging Face Hub

## Requirements
Before running the project, make sure you have the following installed:
- Python 3.8+
- PyTorch
- Hugging Face Diffusers library
- Additional dependencies from the `examples/text_to_image/requirements.txt` file

## Installation
1. Clone the Diffusers repository:
    ```bash
    git clone https://github.com/huggingface/diffusers
    cd diffusers
    ```

2. Install the Diffusers library:
    ```bash
    pip install .
    ```

3. Write the Accelerate configuration:
    ```python
    from accelerate.utils import write_basic_config
    write_basic_config()
    ```

4. Log in to Hugging Face:
    ```python
    from huggingface_hub import notebook_login
    notebook_login()
    ```

5. Navigate to the example folder and install additional requirements:
    ```bash
    cd examples/text_to_image
    pip install -r requirements.txt
    ```

## Training
Run the training script tuturial from : https://huggingface.co/docs/diffusers/en/training/lora
