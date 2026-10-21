---
title: "Exploring Contextual Feature Combinations for Prediction of Subjective Thermal Perceptions"
date: 2024-10-01
image: "/images/papers/thermalfeature_teaser.png"
authors: ['Albin Zeqiri', 'Michael Rietzler', 'Enrico Rukzio']
venue: "Companion of the 2024 on ACM International Joint Conference on Pervasive and Ubiquitous Computing"
venue_short: "UbiComp '24"
paper_type: short   # full (default) | short (short paper, late-breaking work, poster)
tags: ["Machine Learning", "Quantitative Research"]
pdf: "https://dl.acm.org/doi/pdf/10.1145/3675094.3678487"
doi: "https://dl.acm.org/doi/10.1145/3675094.3678487"
---

{{< figure src="/images/papers/thermalfeature_teaser.png" >}}

<h2>Abstract</h2>
Thermal attributes in the environment impact well-being, but their inclusion in standard well-being monitoring is challenging due to complex measurement requirements. Industry standards like the Predicted Mean Vote (PMV) index need numerous measures and specialized setups, making large-scale applications impractical. This study investigates predicting thermal perception ratings using only contextual factors. We conducted an ablation study using the Chinese Thermal Comfort Dataset (CTCD) and a Random Forest (RF) classifier to evaluate prediction performance with different contextual feature combinations on five labeling scales. Results showed that omitting measures required for PMV index calculation and relying on contextual features exclusively achieved F1 scores similar to those when including PMV measures. Key predictive factors included daily outdoor temperature and a person's clothing, weight, and age. These findings suggest that leveraging more accessible contextual data to estimate thermal perception ratings is promising, and further research should explore more contextual factors to enhance prediction accuracy and support well-being assessments.
