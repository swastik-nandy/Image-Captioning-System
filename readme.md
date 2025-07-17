#  Barlow Twins + Transformer Decoder for Image Captioning

This repository presents a modular, experimental image captioning pipeline that combines **Barlow Twins self-supervised learning**, **EfficientNetV2-S** as a visual backbone, and a custom **Transformer Decoder** to generate human-like image captions.  
It explores the separation of representation learning and caption generation — a powerful approach for generalizing across domains.

---

##  Highlights

-  **Barlow Twins Pretraining**: Self-supervised learning with projection head (512 → 128), trained on patch-wise visual tokens
-  **EfficientNetV2-S**: Encoder backbone (with projection head **only during pretraining**)
-  **Transformer Decoder**: 6-layer, 8-head, GELU-activated decoder with learnable positional encodings
-  **Custom Tokenizer & Loader**: Token-level caption generation using `word2idx`, `<SOS>`/`<EOS>` logic, with fallback image handling
-  **Dataset**: Microsoft COCO 2017 for both training and evaluation
-  **Fully PyTorch** — no external vision-language libraries used

