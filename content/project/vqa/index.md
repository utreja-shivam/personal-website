---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Visual Question Answering with Neural Nets over Graphs"
summary: "Implemented a method which builds separate graphs over image objects and question words; and then trains a neural network over these graphs for visual question answering."
authors: []
tags: ["NLP", "Neural Networks", "Python", "Pytorch", "NLTK Library"]
categories: []
date: 2022-01-28T13:42:53+05:30

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Pairs of contrasting images that have opposite answers to the same question."
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

Visual question answering (VQA) is an essential method in extracting useful information from image and video data. This type of semantic analysis of visual data can be very pivotal in fields like human-machine interaction and robotics. Most methods on this task handle the language modelling and image modelling tasks separately which loses out on a lot of structural information. This report discusses a different approach, first suggested by Teney et al., in which we build graphs over the image objects and question words. These graphs are then processed with neural networks over graphs in order to capture the un-ordered nature of information in the images and the questions and then finally, identify correlations between the objects and the words most useful to the VQA task.