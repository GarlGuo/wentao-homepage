---
title: 'GraB: Finding Provably Better Data Permutations than Random Reshuffling'

authors:
  - Yucheng Lu
  - Wentao Guo
  - Christopher De Sa


date: '2022-12-01'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2022-12-01'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In Thirty-Sixth Annual Conference on Neural Information Processing Systems
publication_short: In NeurIPS'22

abstract: Random reshuffling, which randomly permutes the dataset each epoch, is widely adopted in model training because it yields faster convergence than with-replacement sampling. Recent studies indicate greedily chosen data orderings can further speed up convergence empirically, at the cost of using more computation and memory. However, greedy ordering lacks theoretical justification and has limited utility due to its non-trivial memory and computation overhead. In this paper, we first formulate an example-ordering framework named herding and answer affirmatively that SGD with herding converges at the rate $$O(T^{-2/3})$$ on smooth, non-convex objectives, faster than the $$O(n^{1/3}T^{-2/3})$$ obtained by random reshuffling, where $$n$$ denotes the number of data points and $$T$$ denotes the total number of iterations. To reduce the memory overhead, we leverage discrepancy minimization theory to propose an online Gradient Balancing algorithm (GraB) that enjoys the same rate as herding, while reducing the memory usage from $$O(nd)$$ to just $$O(d)$$ and computation from $$O(n^2)$$ to $$O(n)$$, where $$d$$ denotes the model dimension. We show empirically on applications including MNIST, CIFAR10, WikiText and GLUE that GraB can outperform random reshuffling in terms of both training and validation performance, and even outperform state-of-the-art greedy ordering while reducing memory usage over $$100\times$$.

tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://proceedings.neurips.cc/paper_files/paper/2022/file/3acb49252187efa352a1ae0e4b066ced-Paper-Conference.pdf'
url_poster: 'https://drive.google.com/file/d/1bElkwm6O5d42qQP0MNN_58cQNoKCf5SW'

image:
  caption: 'The figure illustrates how Reorder algorithm reorders the vectors with Balancing subroutine - the new order is obtained by concatenating original order of the examples with +1, followed by the reverse order of the examples with -1. Image credit: GraB Paper Figure 1'
  focal_point: ''
  preview_only: false
---
