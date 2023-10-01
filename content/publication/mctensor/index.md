---
title: 'MCTensor: A High-Precision Deep Learning Library with Multi-Component Floating-Point'

authors:
  - Tao Yu
  - Wentao Guo
  - Jianan Canal Li
  - Tiancheng Yuan
  - Christopher De Sa

# Author notes (optional)
author_notes:
  - 'Equal contribution'
  - 'Equal contribution'
  - 'Equal contribution'
  - 'Equal contribution'

date: '2022-06-15'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2022-06-15'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['article']

# Publication name and optional abbreviated publication name.
publication: In Hardware-aware Efficient Training Workshop in The Thirty-ninth International Conference on Machine Learning
publication_short: In HAET workshop at ICML'22

abstract: In this paper, we introduce MCTensor, a library based on PyTorch for providing general-purpose and high-precision arithmetic for DL training. MCTensor is used in the same way as PyTorch Tensor. We implement multiple basic, matrix-level computation operators and NN modules for MCTensor with identical PyTorch interface. Our algorithms achieve high precision computation and also benefits from heavily-optimized PyTorch floating-point arithmetic. We evaluate MCTensor arithmetic against PyTorch native arithmetic for a series of tasks, where models using MCTensor in float16 would match or outperform the PyTorch model with float32 or float64 precision.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2207.08867.pdf'
url_poster: 'https://docs.google.com/presentation/d/1cvsQn8ArPN_tHx6Ntw1JrBUy-iJ1HsX1LIGNgCT6Wb0'
url_slide: 'https://docs.google.com/presentation/d/1Gov3DrqyGZZa8whCPPljo1ft42EFRld2y2VopiKVR0I/edit?usp=sharing'
url_video: 'https://youtu.be/uHc4l35z0Vk'
url_source: 'https://github.com/ydtydr/MCTensor'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'MCTensor Loss Curve on a Linear Regression Task. MCTensor with Float16 could achieve higher precision than vanilla PyTorch Float16 and achieves lower train loss upon the convergence of linear regression model. Image credit: MCTensor Paper Figure 1'
  focal_point: ''
  preview_only: false

---
