Fast Stable Diffusion Image Generation
This project provides a streamlined implementation of Stable Diffusion for fast image generation using text prompts. It's optimized for quick execution in Google Colab, aiming to generate images within 3-4 minutes.
Features

Utilizes the Stable Diffusion 2 base model for image generation
Optimized for speed with minimal quality trade-offs
Easily customizable prompts for diverse image generation
Designed to work efficiently in Google Colab environments

Requirements

Python 3.7+
PyTorch 2.0+
Transformers 4.31.0
Diffusers 0.21.4
Accelerate 0.21.0
Matplotlib

Installation
To set up the project, run the following command in a Colab notebook cell:
pythonCopy!pip install diffusers==0.21.4 transformers==4.31.0 accelerate==0.21.0 torch==2.0.1 matplotlib
Usage

Clone this repository or copy the code into a Google Colab notebook.
Ensure you have a Hugging Face account and token. Replace CFG.hf_token with your actual token.
Run the code chunks in order:

Imports and Configuration
Model Initialization
Image Generation Function
Display Function
Main Execution



To generate an image, modify the prompt variable in the Main Execution chunk:
pythonCopyprompt = "your text prompt here"
generated_image = generate_image(prompt, image_gen_model)
display_image(generated_image, prompt)
Configuration
You can adjust various parameters in the CFG class to fine-tune the generation process:

image_gen_steps: Number of inference steps (default: 20)
image_gen_size: Output image size (default: 256x256)
image_gen_guidance_scale: Guidance scale for generation (default: 7.5)

License
This project is open-source and available under the MIT License.
Acknowledgments
This project uses the Stable Diffusion model by Stability AI and the Diffusers library by Hugging Face.
Disclaimer
Please ensure you comply with the Stable Diffusion model's license and usage terms when using this code.
