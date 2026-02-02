## 🎭 Joke-GPT: Building a Transformer from Scratch
A character-level language model built in PyTorch, inspired by Andrej Karpathy's "Zero to Hero" series. 

This project demonstrates an understanding of how Large Language Models (LLMs) function, moving from a simple Bigram baseline to a mini Generative Pre-Trained Transformer (GPT).


# 🚀 Overview
The goal of this project was to train a neural network to understand the linguistic structure of humor—specifically short, one-liner jokes. Unlike using pre-trained models (like GPT-4), this model was built from the ground up, including the implementation of self-attention mechanisms and training loops.

# 🛠️ Tech Stack
Language: Python

Framework: PyTorch

Environment: Google Colab (GPU Accelerated)

Dataset: Short Jokes Dataset (~230k samples)

🏗️ Architectural Features
The model implements the following core concepts of the Transformer architecture:

Self-Attention: Single-head and Multi-head attention mechanisms to capture long-range dependencies in text.

Residual Connections & LayerNorm: To stabilize deep network training and prevent vanishing gradients.

Positional Encodings: Providing the model with a sense of sequence order in a non-sequential architecture.

Feed-Forward Networks: Position-wise MLPs to process the information gathered via attention.

📈 Learning Progression
I structured the development into two distinct phases to measure performance gains:

The Bigram Baseline: A simple lookup table model that predicted the next character based solely on the current one.

The Transformer: A multi-layered attention-based model that utilized context (block_size) to maintain the "Setup ➡️ Punchline" structure.

📊 Key Results
Loss Function: Cross-Entropy Loss

Final Validation Loss: [Insert your final val loss here, e.g., 1.45]

Hardware: Trained using a free NVIDIA T4 GPU on Google Colab.

📝 How to Use
Open the .ipynb file in Google Colab.

Ensure the Hardware Accelerator is set to T4 GPU.

Run all cells to preprocess the data, define the architecture, and begin the training loop.

Use the generate function at the bottom to see the model's attempt at comedy!
