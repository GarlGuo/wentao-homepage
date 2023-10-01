---
title: 'CD-GraB: Coordinating Distributed Example Orders for Provably Accelerated Training'

authors:
  - A. Feder Cooper
  - Wentao Guo
  - Khiem Pham
  - Tiancheng Yuan
  - Charlie F. Ruan
  - Yucheng Lu

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
  caption: 'Image credit: [CD-GraB Algorithm](cd-grab/PairBalance.drawio.jpg)'
  focal_point: ''
  preview_only: false

---
