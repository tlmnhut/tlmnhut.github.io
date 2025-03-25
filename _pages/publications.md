---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

You can find my papers on [my Google Scholar profile](https://scholar.google.com/citations?user=vs1cgLcAAAAJ&hl=en).

Plus the conference abstracts:
1. **Truong, N.**, & Hasson, U. (2025). *Weight-similarity Topographic Networks Improve Retinotopy and Noise Robustness.*
Journal of Vision. [[html]](https://www.visionsciences.org/presentation/?id=2208)
2. **Truong, N.**, & Hasson, U. (2024). *Pruning sparse features for cognitive modeling.*
In Conference on Cognitive Computational Neuroscience 2024. [[pdf]](https://2024.ccneuro.org/pdf/82_Paper_authored_CCN_2024.pdf)
3. **Truong, N.**, Bavaresco, A., & Hasson, U. (2023). *The Impact of Rarely-firing Nodes in Neural Networks on Representational Geometry and Predictions of Human Similarity Judgments.*
In Conference on Cognitive Computational Neuroscience 2023 (pp. 1025-1028). [[pdf]](https://iris.unitn.it/bitstream/11572/389329/1/0001025.pdf)
4. **Truong, N.**, Bavaresco, A., & Hasson, U. (2023). *Unsupervised feature selection methods for modeling human similarity judgments with deep neural networks.*
Journal of Vision, 23(9), 4975-4975. [[html]](https://jov.arvojournals.org/article.aspx?articleid=2791536)

{% comment %}
{% if site.author.googlescholar %}

  <div class="wordwrap">You can also find my articles on <a href="{{https://webapps.unitn.it/du/en/Persona/PER0220509/Pubblicazioni}}">my university profile</a>.</div>

{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}

  {% include archive-single.html %}

{% endfor %}
{% endcomment %}