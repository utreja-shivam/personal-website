---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Story Generation Using Independent Plot Points"
summary: "Implemented statistical machine translation and plot graphs method for generating a coherent story from given independent plot points. The method using plot graphs performed much better, but the context of stories was very limited."
authors: []
tags: ["NLP", "Python", "NLTK Library"]
categories: []
date: 2022-01-28T13:42:53+05:30

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "An example album from the Visual Storytelling Dataset."
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

Story generation has always been associated with creative minds and sound writers. However, with advancements in neural networks and learning algorithms, it has now become possible for computers to mimic writing styles and synthesise stories. Our work requires the AI agent to finish stories based on open plot lines supplied to it. The only constraint is that the story should be coherent and readable.

## Problem Statement

We aim to generate a logically coherent story through intermediate plot points.We intend to use a possible combination of the two approaches mentioned in literature review as per their merits. The dataset description of each of these approaches are also given in the following sections. Story Generation is perceived in many different ways today. We have worked on two different approaches as follows:

**Approach I**

Coherent story generation from independent descriptions, describing a scene or an event.

**Approach II**

Automatically selecting a sequence of events that meet a set of criteria and can be told as a story.
Knowledge-intensive: Rely on a priori defined domain models about fictional worlds, including characters, places, and actions that can be performed.