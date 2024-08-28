---
title: 'Ranking with Slot Constraints'

authors:
  - Wentao Guo
  - Andrew Wang
  - Bradon Thymes
  - Thorsten Joachims

author_notes:
  - 'Equal contribution'
  - 'Equal contribution'

date: '2024-08-24'
doi: '10.1145/3637528.3672000'

# Schedule page publish date (NOT publication's date).

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication: Proceedings of the 30th ACM SIGKDD Conference on Knowledge Discovery and Data Mining
publication_short: KDD'24

abstract: Rankings are increasingly used as part of human decision-making processes to most effectively allocate reviewing resources. Many of these processes have complex constraints, and we identify slot constraints as a model for a wide range of application problems -- from college admission with limited slots for different majors, to composing a stratified cohort of eligible participants in a medical trial. In this paper, we formalize the slot-constrained ranking problem as producing a ranking that maximizes the number of filled slots if candidates are evaluated by a human decision maker for slot eligibility in the order of the ranking. We show that naive adaptations of the Probability Ranking Principle (PRP) can be highly sub-optimal for slot-constrained ranking problems, and we devise a new ranking algorithm, called MatchRank. MatchRank generalizes the PRP, and it subsumes the PRP as a special case when there are no slot constraints. Our theoretical analysis shows that MatchRank has a strong approximation guarantee without any independence assumptions between slots or candidates. Furthermore, we show how MatchRank can be implemented efficiently. Beyond the theoretical guarantees, empirical evaluations show that MatchRank can provide substantial improvements over a range of synthetic and real-world tasks.

tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://dl.acm.org/doi/pdf/10.1145/3637528.3672000'
url_poster: 'https://docs.google.com/presentation/d/1ZBuVVF9oPMh_9pQH1T1hnaWvAddGP8-K/edit?usp=sharing&ouid=102786752493620407928&rtpof=true&sd=true'
url_slide: 'https://docs.google.com/presentation/d/1CAR7mm69Vu9nm-nkCA68XGfzVdmlaZyV/edit?usp=sharing&ouid=102786752493620407928&rtpof=true&sd=true'
url_code: 'https://github.com/GarlGuo/ranking_with_slot_constraints'

image:
  caption: 'The figure illustrates the ranking framework that our paper considers.'
  focal_point: ''
  preview_only: false
---
