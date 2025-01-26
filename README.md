# LLM GGUF Auto Converter

An automated Jupyter notebook solution for converting and quantizing Large Language Models to GGUF format. This tool streamlines the process of converting models from Hugging Face to GGUF format with multiple quantization options. It was inspired by Maxime Labonne script but 
that one was not working for me and was in Google Colab. 

## Features

- Automated conversion process
- Batch processing of multiple quantization formats (Q2_K to Q8_0)
- Automatic CUDA detection and utilisation
- Integrated Hugging Face upload functionality
- Progress tracking for long conversions
- Automatic model card generation
- Built on llama.cpp for optimal performance

## Supported Quantization Methods

All standard llama.cpp quantization methods are supported:
- Q2_K: Ultra-lightweight (2-bit)
- Q3_K_M: Balanced lightweight (3-bit)
- Q4_K_M: Standard balanced (4-bit)
- Q5_K_M: Enhanced balanced (5-bit)
- Q6_K: High quality (6-bit)
- Q8_0: Maximum quality (8-bit)

## Prerequisites

- Python 3.8+
- Jupyter Notebook environment
- CUDA capable GPU
- Hugging Face account and API token
- CMake
- Git

## Configuration

Before running the notebook, update these 3 required variables:

```python
# The Hugging Face model ID to convert (e.g., "mistralai/Mistral-7B-v0.1")
MODEL_ID = "your-model-id-here"

# Your Hugging Face username
USERNAME = "your-username"

# Your Hugging Face API token from https://huggingface.co/settings/tokens
HF_TOKEN = "your-token-here"
```
## Quick Start

1. Clone this repository
2. Open the Jupyter notebook
3. Update the configuration variables with your details
4. Run all cells
