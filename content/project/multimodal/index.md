---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Multimodal Sentiment Classification"
summary: "Experimented with several state of the art unimodal and multimodal neural nets to identify sentiment using both, visual and textual modalities. Achieved 70.42% accuracy on hateful meme detection and 88.25% on sarcastic tweet detection (using ViLBERT and MMBT respectively)."
authors: []
tags: ["NLP", "Python", "Pytorch", "Transformers"]
categories: []
date: 2022-01-28T13:42:53+05:30

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "These images depict the Hateful memes and their confounders. Multimodal hateful memes (left), benign image confounders (middle) and benign text confounders (right)."
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
## Introduction

With the world connecting all over social media platforms, expressing emotions through multimodal means has increasingly dominated billions of lives. Hate and disinformation on these platforms is also increasingly multimodal. Some of the most toxic or harmful user content comes in the form of images and videos, accompanied with text.

Memes form a large chunk of traffic on social media platforms. While most of these are harmless and funny in nature, malicious users can use clever combinations of independently innocent images and text to form what may be called “hateful memes” - memes that denigrate people based on qualities such as religion, ethnicity, gender, political alignment etc. As a naive example, a harmless picture of a desert could be combined with the harmless text “Look how many people love you”; making the sentiment of the meme “hateful” as a whole. Automatic detection and removal of such content from social media is a top concern for firms like Facebook and Twitter.

Memes often require a bit of parsing and thinking to get at their meaning, even for reasonably savvy humans, indicating that it’s a much harder problem for AI algorithms. They’re often highly contextual, referential, ironic, and nuanced. They can also be cryptic and encoded so that only members of some specific enclave of internet users can parse their meaning.

On similar lines, sarcasm is no longer a purely linguistic phenomenon. To detect sarcasm, context needs to be taken from both text and image. With the rapid growth of social media usage, multimodal sarcastic tweets are very popular. In such tweets, there is a small text and contrast is shown using an image. For example: The tweet “Perfect flying weather for April” seems normal but when the image of downpour outside the airplane window is added it becomes sarcastic.

Despite the recent breakthroughs in NLP with BERT and related language models, detecting hate and sarcasm in memes/posts continues to pose a challenge due to its inherent multimodal nature. The model needs to be able to make a combined inference on the visual and textual components of the input in order to correctly identify the underlying sentiment.