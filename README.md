# GPT-2 Training and Text Generation
This repository contains Python code for training a GPT-2 model on a given dataset, loading a pre-trained GPT-2 model and tokenizer, and generating text using a pre-trained GPT-2 model.

## Table of Contents
1. Installation
2. Usage

# Installation
To run this code, you can run it on [Google Colab.](https://colab.research.google.com/github/Disciplined-22/gpt_2train_1/blob/main/gpt2_1.ipynb) 

## Required Python libraries.
1. !pip install -U accelerate
2. !pip install -U transformers
3. !pip install transformers[torch]
4. !pip install accelerate -U

# Usage

File Paths
file_path = "/content/drive/MyDrive/gpt_1/gpt_sub_1/neural.txt"
output_dir = '/content/drive/MyDrive/gpt_1/gpt_sub_2'

Change the file path to your drive's folder
The "file_path" directs to .txt file that contents the data or the context.
The "output_dir" directs to another folder which would be used to save the tokenizer and model data in the directory.

The main functions in this repository are:

train: This function trains a GPT-2 model on a given dataset.
load_model: This function loads a pre-trained GPT-2 model from a given path.
load_tokenizer: This function loads a pre-trained GPT-2 tokenizer from a given path.
generate_text: This function generates text using a pre-trained GPT-2 model.
You can import these functions into your own Python scripts to use them. 

from gpt2 import train, load_model, load_tokenizer, generate_text

# Train a model
train('path/to/train/file', 'gpt2', 'path/to/output/dir', True, 8, 50, 50000)

# Load a model
model = load_model('path/to/model')

# Load a tokenizer
tokenizer = load_tokenizer('path/to/tokenizer')

# Generate Text
generate_text(model_path, sequence, max_length):
