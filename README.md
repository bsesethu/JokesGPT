# 🎭 Joke-GPT: Building a Transformer from Scratch
A character-level language model built in PyTorch, inspired by Andrej Karpathy's "Zero to Hero" series. This project demonstrates an understanding of how Large Language Models (LLMs) function, moving from a simple Bigram baseline to a mini Generative Pre-Trained Transformer (GPT).


## 🚀 Overview
The goal of this project was to train a neural network to understand the linguistic structure of humor, specifically short, one-liner jokes. This model was built from the ground up, including the implementation of self-attention mechanisms and training loops.

## 🛠️ Tech Stack
Language: Python

Framework: PyTorch

Environment: Google Colab (GPU Accelerated)

Dataset: Short Jokes Dataset (~3000 samples)

## 📈 Learning Progression
I structured the development into three distinct phases to measure performance gains:

The Bigram Baseline: A simple lookup table model that predicted the next character based solely on the current one.

The Transformer: A multi-layered attention-based model that utilized context (block_size) to maintain the "Setup ➡️ Punchline" structure.

The Transformer with Multiple Heads: Added 4 - 6 Heads, instead of the single head baseline.

📊 Key Results
Loss Function: Cross-Entropy Loss

Final Validation Loss: 1.53

Hardware: Trained using a free NVIDIA T4 GPU on Google Colab.

📝 How to Use
Open the .ipynb file in Google Colab.

Set the Hardware Accelerator to T4 GPU. It runs on CPU as well albeit slower.

Run all cells to preprocess the data, define the architecture, and begin the training loop.

Use the generate function at the bottom of each section to see the model's attempt at comedy!


## Author: Sesethu M. Bango

## Linkedin: https://www.linkedin.com/in/sesethu-bango-197856380
