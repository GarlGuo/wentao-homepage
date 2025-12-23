---
title: 'Zeroth-Order Fine-Tuning of LLMs with Transferable Static Sparsity'

authors:
  - Wentao Guo
  - Jikai Long
  - Yimeng Zeng
  - Zirui Liu
  - Xinyu Yang
  - Yide Ran
  - Jacob R. Gardner
  - Osbert Bastani
  - Christopher De Sa
  - Xiaodong Yu
  - Beidi Chen
  - Zhaozhuo Xu

date: '2025-01-22'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2025-01-22'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: The Thirteenth International Conference on Learning Representations
publication_short: ICLR'25.

abstract: Zeroth-order optimization (ZO) is a memory-efficient strategy for fine-tuning Large Language Models using only forward passes. However, applying ZO fine-tuning in memory-constrained settings such as mobile phones and laptops remains challenging since these settings often involve weight quantization, while ZO requires full-precision perturbation and update. In this study, we address this limitation by combining static sparse ZO fine-tuning with quantization. Our approach transfers a small, static subset (0.1%) of "sensitive" parameters from pre-training to downstream tasks, focusing fine-tuning on this sparse set of parameters. The remaining untuned parameters are quantized, reducing memory demands. Our proposed workflow enables efficient ZO fine-tuning of an Llama2-7B model on a GPU device with less than 8GB of memory while outperforming full model ZO fine-tuning performance and in-context learning.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://openreview.net/pdf?id=myYzr50xBh'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'Image credit: Paper Figure 4'
  focal_point: ''
  preview_only: false
---
