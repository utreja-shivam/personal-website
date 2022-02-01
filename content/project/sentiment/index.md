---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Real Time Sentiment Analysis"
summary: "Designed a machine learning algorithm that uses a convolutional neural network to detect the emotion of a facial image input. The output is one emotion out of a set of 7 possible emotions. Best performance achieved was a top 2 precision of 71%."
authors: []
tags: ["Computer Vision", "Python", "OpenCV", "Tensorflow"]
categories: []
date: 2022-01-28T13:42:53+05:30

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Sample images used to detect underlying sentiment of the person."
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
## Problem Statement

We aim to develop a user-end application to get time-mapped viewer sentiment while watching a video from the following set of 6 different emotions:

E = {neutral, happy, sad, angry, surprised, fearful}

The input will be the real time viewer’s webcam feed while watching the video and the output will be an emotion specified at regular time intervals throughout the video.

## Motivation

- **Widespread need of genuine user feedback**

Users are exposed to a lot of visual content online on a daily basis. This could be in the form of product advertisements, youtube videos, movie trailers etc. The creators of these will be benefited immensely if given the user’s emotional feedback on being exposed to this content. The recommendation systems will also be able to use this data in order to make better recommendations in the future to the same user. This will hence, improve the experience of the consumers, and also provide with constructive feedback to the creators.

- **Drawbacks of the current user review methods**

Presently, the only methods by which creators can get reviews of their content online are via comments, reaction buttons, reviews, feedback forms etc.. There are two major disadvantages of all these methods. Firstly, only a small percentage of users opt to fill these out (which itself is a biased set of users in the first place), of which, an even smaller percentage coincides well with the true feelings of the reviewer, since the reviews can also be affected by external factors[1]. Secondly, these responses are not real-time, but an overall summarized response of what the user thinks he felt of the content as a whole, after watching it completely. This provides a very crude feedback to the creators as well as the recommendation systems to be of any significant use.

- **Advantages of Realtime Sentiment Analysis**

Ideally, the recommendation systems and creators will be benefitted the most if they could know the responses of the users exposed to a given piece of content. These are the pure sentiments that each specific user had exhibited throughout the duration of the video. This data set would be a lot richer, being the time-mapped review of the video. It would also be a lot larger, and less biased as it would be inclusive of all the users watching that specific content. It would also be a highly accurate estimate of the true user emotions, as opposed to what the user chooses to mention in his/her written review.