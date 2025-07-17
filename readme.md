# 🧠 Barlow Twins + Transformer Decoder for Image Captioning

An experimental research pipeline combining **Barlow Twins** self-supervised learning, **EfficientNetV2-S** as a visual backbone, and a **Transformer Decoder** for generating high-quality image captions. This project aims to explore the effectiveness of decoupled visual and language representations for multimodal tasks.

---

## 🚀 Project Overview

This repository proposes a two-phase approach for image captioning:

1. **Self-Supervised Visual Representation Learning**  
   Train an image encoder using [Barlow Twins](https://arxiv.org/abs/2103.03230) to extract powerful features without any labels.

2. **Caption Generation with a Transformer Decoder**  
   Use a transformer-based decoder to generate text descriptions from the visual features extracted by the encoder.

The overall objective is to assess whether self-supervised learning (SSL) can produce image embeddings that rival or exceed traditional supervised setups for vision-language tasks.

---

## 🧪 Key Features

- 🧬 **Barlow Twins** contrastive learning for redundancy-reducing SSL
- ⚡ **EfficientNetV2-S** as a compact and efficient vision backbone
- 🧠 **Transformer Decoder** to generate natural language captions
- 🧪 **Modular Pipeline** with flexible training and evaluation
- 🧪 **Dataset**: [MS COCO 2017](https://cocodataset.org/#download)

---

## 🗂️ Repository Structure

