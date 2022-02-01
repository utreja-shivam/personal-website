---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Identifying Tennis Strokes from Video "
summary: "Implemented variations of recurrent and convolutional neural architectures for fine-tuned action classification in tennis, just using the player’s video. Achieved best average accuracy of 60% across 12 tennis strokes."
authors: []
tags: ["Computer Vision", "Python", "Tensorflow", "OpenCV"]
categories: []
date: 2022-01-28T13:42:53+05:30

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Subjects performing different shots in the
THETIS dataset"
  focal_point: "Center"
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
- name: Poster
  url: uploads/poster-tennis.pdf
  # icon_pack: fab
  # icon: twitter

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

Sports is a field with a huge abundance of high quality visual data. This data holds immense potential to be utilized with the state of the art techniques from computer vision and artificial intelligence, for a variety of tasks. One such task is of action recognition. In the general action recognition task in computer vision, each individual action is highly distinct and the action categories are coarse-grained. However, identifying different actions within a single sport requires a much more fine-tuned action categorization. This project’s main goal was to make an open source implementation of one such model, which recognizes fine-grained action categories in tennis, given the video input of the player. This was followed by experiments with the architecture choice, feature choice and finally, comparison of sequential processing of an LSTM with the time-independent processing, by a pre-trained CNN.