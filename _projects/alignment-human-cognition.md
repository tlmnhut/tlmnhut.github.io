---
title: "Alignment of AI models with human cognition"
years: "2023 – present"
order: 2
summary: >-
  Using pruning techniques and explainable AI to study how deep neural network representations align
  with human similarity judgments, and to identify the visual features humans rely on to compare objects.
papers:
  - authors: "**Truong, N.**, Pesenti, D., & Hasson, U."
    title: "Explaining human comparisons using alignment-importance heatmaps"
    venue: "Computational Brain & Behavior"
    year: 2025
    featured: true
    links:
      doi: "https://doi.org/10.1007/s42113-025-00235-x"
  - authors: "Tarigopula, P., Fairhall, S., Bavaresco, A., **Truong, N.**, & Hasson, U."
    title: "Improved prediction of behavioral and neural similarity spaces using pruned DNNs"
    # Crossref records this as published in print November 2023 (vol. 168, pp. 89-104),
    # not 2024 as originally given -- flagged to Nhut, using the verified date here.
    venue: "Neural Networks"
    year: 2023
    featured: true
    links:
      doi: "https://doi.org/10.1016/j.neunet.2023.08.049"
  - authors: "Bavaresco, A., **Truong, N.**, & Hasson, U."
    title: "Modeling human concepts with subspaces in deep vision models"
    venue: "ACM Transactions on Interactive Intelligent Systems (TIIS)"
    year: 2025
    links:
      doi: "https://doi.org/10.1145/3768340"
  - authors: "**Truong, N.**, & Hasson, U."
    title: "Pruning sparse features for cognitive modeling"
    venue: "Conference on Cognitive Computational Neuroscience (CCN)"
    year: 2024
    links:
      pdf: "https://2024.ccneuro.org/pdf/82_Paper_authored_CCN_2024.pdf"
  - authors: "**Truong, N.**, Bavaresco, A., & Hasson, U."
    title: "The impact of rarely-firing nodes in neural networks on representational geometry and predictions of human similarity judgments"
    venue: "Conference on Cognitive Computational Neuroscience (CCN)"
    year: 2023
    links:
      pdf: "https://iris.unitn.it/bitstream/11572/389329/1/0001025.pdf"
  - authors: "**Truong, N.**, Bavaresco, A., & Hasson, U."
    title: "Unsupervised feature selection methods for modeling human similarity judgments with deep neural networks"
    venue: "Journal of Vision, 23(9)"
    year: 2023
    links:
      html: "https://jov.arvojournals.org/article.aspx?articleid=2791536"
---

A deep vision model and a person can agree on which images look similar while arriving there by
quite different routes. This line of work asks which parts of a network's representation actually
carry the agreement.

The method is subtractive. Pruning units — particularly the rarely-firing ones that contribute
little to a network's output — changes representational geometry in ways that can be measured
against human similarity judgments. Where pruning leaves the match to human behavior intact, the
removed units were not what the alignment rested on. The same framing extends to locating
human-interpretable concepts as subspaces inside a model's representation.
