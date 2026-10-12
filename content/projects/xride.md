---
draft: true
title: "XRIDE: Extended Reality in Transit Dataset for Interaction Techniques in Stationary and Moving Vehicles"
date: 2026-10-07
authors: ['Markus Sasalovici*', 'Albin Zeqiri*', 'Mark Colley', 'Robin Connor Schramm', 'Enrico Rukzio', 'Christian Winkler']
work_in_progress: true
summary: "A multimodal dataset (24 participants, 23.4 h) of XR selection interactions in stationary and moving vehicles, with benchmarks for ML-based selection offset prediction and correction."
tags: ["Machine Learning", "Field Studies", "Quantitative Research", "Extended Reality", "Automotive & Mobility"]
---

<h2>About this project</h2>
Understanding user interactions with extended reality (XR) interfaces in dynamic environments is critical, as vehicle motion can significantly influence interaction precision, usability, and overall user experience. This work presents the XRIDE dataset, which captures how external forces, such as G-forces, vibrations, and varying road conditions, impact interaction performance. In a field study with 24 participants, we recorded four XR interaction methods (Gaze&Pinch, DirectTouch, Handray, and HeadGaze) during a Fitts' Law task in stationary and moving vehicles, yielding 23.4 h of multimodal recordings paired with synchronized vehicle dynamics and annotated road, curve, and maneuver types. Across three experiments, we provide an initial benchmark for selection offset prediction and correction and examine how movement and interaction scenarios affect prediction performance. Using a CatBoost regressor, 84.06% of initially unsuccessful DirectTouch selections could be corrected.
