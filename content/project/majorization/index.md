---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Majorization-Minimization in Large Scale ML"
summary: "Performed theoretical convergence analysis of Incremental MajorizationMinimization for machine learning problems. Implemented the same for both, convex and non-convex objective functions."
authors: []
tags: ["Other", "Python", "Scipy", "Numpy"]
categories: []
date: 2022-01-28T13:42:53+05:30

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
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
One of the crucial problems in machine learning is optimizing sum of functions. Majorization-minimization(MM) is a very popular algorithm and often used due to its convergence guarantees even in non-convex cases (with some assumptions). However, its scalability is still an issue. With increasing data, several stochastic optimization algorithms have been developed to deal with the scale. But most of these algorithms suffer from slow convergence. We therefore present a scalable version of majorization-minimization, particularly focusing on “MISO” algorithm by J. Marial and analyze its convergence. We also compare it with state of the art algorithms and present our insights.