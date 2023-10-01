---
title: 'CD-GraB: Coordinating Distributed Example Orders for Provably Accelerated Training'

authors:
  - A. Feder Cooper
  - Wentao Guo
  - Khiem Pham
  - Tiancheng Yuan
  - Charlie F. Ruan
  - Yucheng Lu
  - Christopher De Sa

# Author notes (optional)
author_notes:
  - 'Equal contribution, alphabetical order'
  - 'Equal contribution, alphabetical order'
  - 'Equal contribution, alphabetical order'

date: '2023'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2023'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In Thirty-Seventh Annual Conference on Neural Information Processing Systems
publication_short: In NeurIPS'23

abstract: Recent research on online Gradient Balancing (GraB) has revealed that there exist permutation-based example orderings that are guaranteed to outperform random reshuffling (RR). Whereas RR arbitrarily permutes training examples, GraB leverages stale gradients from prior epochs to order examples — achieving a provably faster convergence rate than RR. However, GraB is limited by design. While it demonstrates an impressive ability to scale-up training on centralized data, it does not naturally extend to modern distributed ML workloads. We therefore propose Coordinated Distributed GraB (CD-GraB), which uses insights from prior work on kernel thinning to translate the benefits of provably faster permutation-based example ordering to distributed settings. With negligible overhead, CD-GraB exhibits a linear speedup in convergence rate over centralized GraB and outperforms baselines empirically, including distributed RR, on a variety of benchmark tasks.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2302.00845.pdf'
url_poster: 'https://docs.google.com/presentation/d/1FqOM5P4Mp5WdC54fNvLYnyK8TCRhfqHftg7ayFJrBA8'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'Image credit: CD-GraB Paper Figure 1'
  focal_point: ''
  preview_only: false

---
title: 'GraB: Finding Provably Better Data Permutations than Random Reshuffling'

authors:
  - Yucheng Lu
  - Wentao Guo
  - Christopher De Sa


date: '2022'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2022'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In Thirty-Sixth Annual Conference on Neural Information Processing Systems
publication_short: In NeurIPS'22

abstract: Random reshuffling, which randomly permutes the dataset each epoch, is widely adopted in model training because it yields faster convergence than with-replacement sampling. Recent studies indicate greedily chosen data orderings can further speed up convergence empirically, at the cost of using more computation and memory. However, greedy ordering lacks theoretical justification and has limited utility due to its non-trivial memory and computation overhead. In this paper, we first formulate an example-ordering framework named \emph{herding} and answer affirmatively that SGD with herding converges at the rate $O(T^{-2/3})$ on smooth, non-convex objectives, faster than the $O(n^{1/3}T^{-2/3})$ obtained by random reshuffling, where $n$ denotes the number of data points and $T$ denotes the total number of iterations. To reduce the memory overhead, we leverage discrepancy minimization theory to propose an online Gradient Balancing algorithm (GraB) that enjoys the same rate as herding, while reducing the memory usage from $O(nd)$ to just $O(d)$ and computation from $O(n^2)$ to $O(n)$, where $d$ denotes the model dimension. We show empirically on applications including MNIST, CIFAR10, WikiText and GLUE that GraB can outperform random reshuffling in terms of both training and validation performance, and even outperform state-of-the-art greedy ordering while reducing memory usage over $100\times$.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://proceedings.neurips.cc/paper_files/paper/2022/file/3acb49252187efa352a1ae0e4b066ced-Paper-Conference.pdf'

---
