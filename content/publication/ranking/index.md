---
title: 'Ranking with Slot Constraints'

authors:
  - Wentao Guo
  - Andrew Wang
  - Bradon Thymes
  - Thorsten Joachims


date: '2023-10-27'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2023-10-27'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['article']


abstract: We introduce the problem of ranking with slot constraints, which can be used to model a wide range of application problems -- from college admission with limited slots for different majors, to composing a stratified cohort of eligible participants in a medical trial. We show that the conventional Probability Ranking Principle (PRP) can be highly sub-optimal for slot-constrained ranking problems, and we devise a new ranking algorithm, called MatchRank. The goal of MatchRank is to produce rankings that maximize the number of filled slots if candidates are evaluated by a human decision maker in the order of the ranking. In this way, MatchRank generalizes the PRP, and it subsumes the PRP as a special case when there are no slot constraints. Our theoretical analysis shows that MatchRank has a strong approximation guarantee without any independence assumptions between slots or candidates. Furthermore, we show how MatchRank can be implemented efficiently. Beyond the theoretical guarantees, empirical evaluations show that MatchRank can provide substantial improvements over a range of synthetic and real-world tasks.

tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2310.17870.pdf'

image:
  caption: 'The figure illustrates the 2-stage ranking framework that our paper considers.'
  focal_point: ''
  preview_only: false
---
