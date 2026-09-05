---
title: "Topographic models"
years: "2024 – present"
order: 1
summary: >-
  Deep neural networks that simulate the spatial and functional organization of the brain, built to be
  more biologically plausible models of cognition.
papers:
  - authors: "**Truong, N.**, & Hasson, U."
    title: "Beyond topography: Topographic regularization improves robustness and reshapes representations in convolutional neural networks"
    venue: "Neurocomputing"
    year: 2026
    featured: true
    links:
      doi: "https://doi.org/10.1016/j.neucom.2026.134496"
      arxiv: "https://arxiv.org/abs/2508.00043"
  - authors: "Cortinovis, D., **Truong, N.**, Op de Beeck, H., & Bracci, S."
    title: "Investigating action topography in visual cortex and deep artificial neural networks"
    venue: "Nature Communications"
    year: 2025
    featured: true
    links:
      doi: "https://www.nature.com/articles/s41467-025-67855-6"
  - authors: "**Truong, N.**, & Hasson, U."
    title: "Weight-similarity topographic networks improve retinotopy and noise robustness"
    venue: "Journal of Vision (VSS abstract)"
    year: 2025
    links:
      html: "https://www.visionsciences.org/presentation/?id=2208"
---

Cortex is organized spatially: nearby neurons tend to respond to related things. Standard
convolutional networks have no such constraint — any unit may sit anywhere. Topographic models add
one, so that spatial position in the network carries meaning.

I study what that constraint buys. Adding a weight-similarity term during training produces
retinotopic organization and functional clustering without supervision, and the resulting networks
are measurably more robust to noise. The same lens applies in the other direction: comparing the
topography that emerges in these models against the topography measured in human visual cortex.
