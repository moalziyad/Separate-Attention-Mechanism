# 🧠 GLAB: Generative Human-Like Arabic Brain

![Status](https://img.shields.io/badge/status-research-blue)
![Language](https://img.shields.io/badge/language-Python-yellow)
![Framework](https://img.shields.io/badge/framework-PyTorch-red)
![Focus](https://img.shields.io/badge/focus-Arabic%20NLP-green)
![Model](https://img.shields.io/badge/model-BERT--based-purple)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

## 📌 Overview

GLAB is a tokenization framework designed for root-based languages, with a focus on Arabic.

Traditional tokenizers struggle with Arabic because of morphological complexity, large vocabulary size, and inefficient subword segmentation. GLAB introduces a two-stage encoding architecture that preserves character-level information while learning word-level semantics, reducing sequence length and improving training efficiency.

## 🚨 Problem

Standard tokenizers such as BPE and WordPiece work well for affix-based languages, but they are less effective for root-based languages such as Arabic. This leads to:

- Excessive token fragmentation
- Longer token sequences
- Higher computational cost
- Weaker semantic representation

Arabic contains more than 12 million words derived from root-based patterns.

## 💡 Solution

GLAB uses two encoders:

- Characters-to-Word Encoder
- Words-to-Sentence Encoder

## 🏗️ Architecture

Characters → Character Encoder → Word Embeddings → Context Encoder → Sentence Representation

## 🔤 Tokenization

| Token | Purpose |
|------|---------|
| [CLS] | Sentence representation |
| [SEP] | Separator |
| [UNK] | Unknown |
| [PAD] | Padding |
| [MASK] | Mask |

## 🔄 Pipeline

![Architecture](model_architecture.png)

## 🚀 Key Contributions

- Character-to-sequence tokenization
- Arabic-specific design
- Efficient representation

## 👥 Authors

- Mohammed S. Alziyad  
- Abdullah E. Alsuwaidan  

Supervisor: Dr. Mohammed Alfaki

## 📜 License

MIT License
