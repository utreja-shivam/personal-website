---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Scaling Mixed Membership Stochastic Blockmodels to Large Datasets"
summary: "Explored both, the generative story and inference methods for this probabilistic model for relational data. Also attempted scaling this method to large data-sets by exploring graph sub-sampling techniques and nested variational inference."
authors: []
tags: ["Other", "Probabilistic Modelling"]
categories: []
date: 2022-01-28T13:42:53+05:30

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Convergence observed for Nested Inference on 55*55 graph, K=3. Check paper for details."
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: uploads/slides-stochastic.pdf
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
## Abstract

Relational data is ubiquitious nowadays and models to handle such data are thus important to study. In this project, we explore Mixed Membership Stochastic Blockmodels in detail starting from scratch and exploring ways to achieve scalability over baseline implementations. To better report our results, we implement the baseline approach and a few scalable approaches to MMSB, for a qualitative comparison.

## Problem Statement

Given real-world relational datasets, like the US patent dataset or the dataset on scientific articles; we wish to identify the underlying community structure i.e., clusters of densely connected nodes. In order to do this, we first propose a probabilistic generative story for this kind of data, followed by proposing methods to learn the parameters of this model efficiently.