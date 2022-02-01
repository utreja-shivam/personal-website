---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "One Shot Learning"
summary: "Implemented variations of Siamese networks and Matching networks for one-shot learning on the Omniglot and MNIST datasets. Achieved best accuracy of 85.63% on 20-way one-shot learning task, using the matching network architecture."
authors: []
tags: ["Deep Learning", "Python", "Pytorch"]
categories: []
date: 2022-01-28T13:42:53+05:30

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Training and testing the Siamese network for one-shot learning."
  focal_point: "Center"
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
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
## Abstract

The process of learning good features for machine learning applications can be very computationally expensive and may prove difficult in cases where little data is available. A prototypical example of this is the one-shot learning setting, in which we must correctly make predictions given only a single example of each new class. In this paper, we firstly explore Siamese Networks, a unique twin-network setting which is capable of checking how similar any two inputs are. The observed shortcomings of the model inspire us to explore a more robust model, Matching Networks, a neural network which uses recent advances in attention and memory that enable rapid learning. We then extend the models to the MNIST in addition to the standard Omniglot dataset they are trained on to check their robustness and achieve promising results.