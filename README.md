# Building a Language Model from Scratch

## 📝 Project Overview

This project demonstrates how to build the foundational components of a modern language model (LLM) from scratch, following GPT-style architecture principles. The pipeline covers everything from raw text processing and tokenization to embedding layer implementation and batch data preparation, using PyTorch and tiktoken.

The goal is to provide an educational, hands-on implementation of the core elements behind large language models, focusing on text preprocessing, tokenization, and embedding mechanics.

---

## 🚀 Key Features

- **Custom Dataset Preparation:**  
  Implements a sliding window approach for generating input-target pairs from raw text, with configurable sequence length and stride.
- **Tokenization:**  
  Utilizes Byte Pair Encoding (BPE) via [tiktoken](https://github.com/openai/tiktoken) for efficient subword tokenization.
- **Embedding Layers:**  
  - Token embeddings using PyTorch’s `nn.Embedding`
  - Absolute positional embeddings (GPT-style)
  - Combined token + positional embeddings
- **Batch Processing:**  
  Efficient batch generation using PyTorch’s `DataLoader` and a custom `GPTDatasetV1` class.
- **Experimental Flexibility:**  
  Easily adjust batch size, sequence length, stride, and embedding dimensions for experimentation.
- **Visualization & Verification:**  
  Embedding shape checks and visualizations to ensure correct implementation.

---

## 📚 Key Concepts Covered

- Tokenization and subword units (BPE)
- Sliding window input-target generation
- Embedding layer mechanics and positional encoding
- Batch processing with DataLoader
- Experimental setup for context length and embedding dimension

---

## 📁 Dataset

- **Source:**  
  [the-verdict.txt](#) (downloaded via `urllib`)
- **Description:**  
  Raw text corpus used for training and experimentation.

---

## 🛠️ Dependencies

- **Python 3.x**
- **PyTorch**
- **tiktoken**
- **urllib** (for data download)
