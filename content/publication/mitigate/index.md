---
title: 'Mitigating Non-IID Drift in Zeroth-Order Federated LLM Fine-Tuning with Transferable Sparsity'

authors:
  - Yide Ran
  - Wentao Guo
  - Jingwei Sun
  - Yanzhou Pan
  - Xiaodong Yu
  - Hao Wang
  - Jianwen Xie
  - Yiran Chen
  - Denghui Zhang
  - Zhaozhuo Xu

date: '2026-01-25'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2025-06-03'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: The Fourteenth International Conference on Learning Representations
publication_short: ICLR'26

abstract: "Federated Learning enables collaborative fine-tuning of Large Language Models (LLMs) across decentralized Non-Independent and Identically Distributed (Non-IID) clients, but such models' massive parameter sizes lead to significant memory and communication challenges. This work introduces Meerkat, a sparse zeroth-order optimization (ZO) method designed for federated LLM fine-tuning. By limiting fine-tuning to a transferable, static, extremely sparse subset of parameters, Meerkat achieves remarkable communication efficiency, enabling cost-effective high-frequency synchronization. With theoretical analysis and experiments, we show that this high-frequency communication effectively mitigates Non-IID data challenges and leads to superior performance compared to full-parameter ZO. Furthermore, experiment results show that Meerkat outperforms existing sparsity baselines with better performance at the same communication frequency. To further handle Non-IID drift, Meerkat leverages traceable local updates and forms a virtual path for each client. This virtual path mechanism reveals the GradIP phenomenon : the inner products between LLM pre-training gradients maintained by server and client gradients estimated via ZO converges for extreme Non-IID clients but oscillates for IID ones. This distinct behavior provides a signal for identifying clients with extreme data heterogeneity. Using this signal, Meerkat-vp is proposed to analyze GradIP trajectories to identify extreme Non-IID clients and applies early stopping to enhance aggregated model quality. Experiments confirm that Meerkat and Meerkat-vp significantly improve the efficiency and effectiveness of ZO federated LLM fine-tuning."


tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2506.03337'
---
