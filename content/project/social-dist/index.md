---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Social Distancing App"
summary: "Designed an Android app that combines GPS and Bluetooth information to help the user identify surrounding regions of high human density."
authors: []
tags: ["Mobile Computing", "Android Studio"]
categories: []
date: 2022-01-28T13:42:53+05:30

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "App shows markers based on density of people in immediate vicinity"
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: "https://github.com/utreja-shivam/590U_A5"
url_pdf: ""
url_slides: ""
url_video: "https://drive.google.com/file/d/1HJwab6mBSG171L6l8UbThQ9gEHgP9FT9/view"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
## Idea/Motivation

A large population of the public now-a-days have smartphones. Secondly, almost all smartphones of the present day have bluetooth and GPS capabilities. The GPS gives the users' realtime location, whereas the bluetooth can be used to continiuously discover other bluetooth smartphones (which can easily be used as a proxy for other people nearby!) in the near vicinity. Hence, these sensors when used in sync hold immense potential to apply ubiquituous to the problem of social distancing.

Given the above motivation, we can come up with the following idea for the app;

Use the bluetooth to discover new smartphone devices in close vicinity, while outside home, at constant intervals of time (every 10 to 15mins). Combine this with the realtime location data to identify crowded regions on a map and provide this info to the user in realtime. Lastly, utilize the average count of bluetooth devices seen throughout the day as a logical metric for social distancing.