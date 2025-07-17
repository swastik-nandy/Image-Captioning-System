# 🧠 Barlow Twins + Transformer Decoder for Image Captioning

## This project is part of an ongoing experimental research effort exploring how self-supervised visual features (via Barlow Twins) can be used effectively with Transformer-based decoders for image     captioning tasks. The encoder is built on EfficientNetV2-S, with a projection head during pretraining. The decoder is a custom Transformer stack.

⚠️ Note: This repository is not production-ready. It is under active development and research.
I'm actively seeking guidance, feedback, and open to collaborations from the community.

This repository presents a modular, experimental image captioning pipeline that combines **Barlow Twins self-supervised learning**, **EfficientNetV2-S** as a visual backbone, and a custom **Transformer Decoder** to generate human-like image captions.  
It explores the separation of representation learning and caption generation — a powerful approach for generalizing across domains.

---

## 🚀 Highlights

- 🧬 **Barlow Twins Pretraining**: Self-supervised learning with projection head (512 → 128), trained on patch-wise visual tokens
- ⚡ **EfficientNetV2-S**: Encoder backbone (with projection head **only during pretraining**)
- 🧠 **Transformer Decoder**: 6-layer, 8-head, GELU-activated decoder with learnable positional encodings
- 📝 **Custom Tokenizer & Loader**: Token-level caption generation using `word2idx`, `<SOS>`/`<EOS>` logic, with fallback image handling
- 📦 **Dataset**: Microsoft COCO 2017 for both training and evaluation
- ⚙️ **Fully PyTorch** — no external vision-language libraries used
