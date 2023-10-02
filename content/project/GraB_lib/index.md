---
title: GraB-sampler - provably better data orderings meets PyTorch
summary: We implement a library named `GraB-sampler` that will obtain a good data orderings during training while compatible with PyTorch's `torch.utils.data.DataLoader`.

tags:
  - Data orderings
  - Machine learning
  - Optimization

date: '2023-05-31'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: All balancing subroutines will reach O(1) herding bound in theory.
  focal_point: Smart

url_code: 'https://github.com/garywei944/grab-sampler'

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

Inspired by our [CD-GraB](https://arxiv.org/pdf/2302.00845.pdf) and [GraB](https://proceedings.neurips.cc/paper_files/paper/2022/file/3acb49252187efa352a1ae0e4b066ced-Paper-Conference.pdf) paper, we implement a library named `GraB-sampler` that will obtain a good data orderings during training while compatible with PyTorch's `torch.utils.data.DataLoader`. The library could be found [here](https://github.com/garywei944/grab-sampler). Besides the `PairBalance` in CD-GraB and `MeanBalance` in GraB paper, we also develop a **recursive balancing** subroutines as follows. ![RecursiveMeanBalance reorders example repeatedly from top to down in the accumulator tree](recursiveBalance.jpg)

The high-level idea behind the recursive balancing algorithm is that both `PairBalance` and `MeanBalance` requires 2 components: balancing procedure and an accumulator, and we could build a tree of accumulator and call the balancing procedure recursively across each level of the accumulator tree. Each time once we obtain a sign of `+1` or `-1`, we proceed to the next level of tree and re-call the corresponding balancing subroutine.

This recursive balancing algorithm will reach O(1) herding bound in a much faster speed, as shown in the <span style="color: green;">green</span> and <span style="color: red;">red</span> lines below. ![The herding bound of RecursiveMeanBalance is much faster than MeanBalance.](featured.jpg)
