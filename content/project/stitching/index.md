---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Image Stitching using SIFT Features"
summary: "Implemented an image stitching method which first, detects keypoints in the two images using a blob detector and SIFT features. It then uses these keypoints to perform the RANSAC algorithm, which estimates the best affine transform between the pairs of images."
authors: []
tags: ["Computer Vision", "Python", "OpenCV", "Scipy", "Numpy"]
categories: []
date: 2022-01-28T13:42:53+05:30

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Left: Matched SIFT features using RANSAC. Right: Stitched images output."
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
