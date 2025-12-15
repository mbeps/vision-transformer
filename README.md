# **Vision Transformer**

A compact implementation of a Vision Transformer (ViT).
The code is written for learning and experiments.

# Features

- Minimal ViT from scratch.
- Patch embedding via conv projection.
- Transformer encoder stack with multi-head attention.
- Training and evaluation loops.
- Prediction grid visualization for qualitative checks.

# Design

The code follows small, clear modules.
Each part maps to a ViT concept.

- `PatchEmbedding`: turns image into tokens.
- `TransformerEncoderLayer`: attention + MLP + residuals.
- `VisionTransformer`: stacks encoders and adds head.
- Training and evaluation utilities are separate.

# Stack

- [Python](https://www.python.org/) — Language used for code.
- [PyTorch](https://pytorch.org/) — Deep learning framework.
- [torchvision](https://pytorch.org/vision/stable/) — Datasets and transforms.
- [matplotlib](https://matplotlib.org/) — Plotting and visualization.

# Requirements

- Python 3.12 or newer.

# Running Locally
Clone the repository:
```sh
git clone git@github.com:mbeps/vision-transformer.git
```

Install dependencies using UV:
```bash
uv sync
```

Run the notebook `notebook.ipynb` to train and test the model.

# References

- [An Image is Worth 16x16: Transformers for Image Recognition at Scale](https://arxiv.org/abs/2010.11929)
- [Attention Is All You Need](https://arxiv.org/abs/1706.03762)
- [PyTorch](https://pytorch.org/)
- [torchvision](https://pytorch.org/vision/stable/)
- [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html)
