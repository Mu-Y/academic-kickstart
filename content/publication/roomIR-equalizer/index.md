---
title: "Digital Room Correction using Parallel Second-order Filter-based Equalizer"
authors: ["**Mu Yang**"]
date: "2018-04-20"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: ""

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
#publication_types: ["4"]

# Publication name and optional abbreviated publication name.
publication: "*USC course EE522: Immersive Audio Processing*"
publication_short:

abstract: "Room Acoustics matters. Producers in studio need to monitor every subtle detail in music. Every ordinary people wants excellent sound quality for their playback system to enjoy movies, music, TV broadcast, etc. However, if the room where the sound system is installed produces undesired acoustic effects (e.g. reverbration), these wishes could never come true, no matter how much money you invest in your electronic playback system. Bad room acoustics is a common problem in almost every realistic room. That is why we need extra calibration technologies to make up for the room acoustics, or to put it more specifically, the frequency response of the room. In this project, a Parallel second-order-based equalizer design method is deployed for loudspeaker-room correction. "

# Summary. An optional shortened abstract.
summary: "A Parallel second-order-based equalizer for Room Impulse Response Calibration."

tags:
- proj
featured: true

links:
- name: Audio Samples
  url: https://mu-y.github.io/speech_samples/roomIR/
url_pdf: 'https://github.com/Mu-Y/RoomIR-equalizer/blob/master/final_report.pdf'
url_code: 'https://github.com/Mu-Y/RoomIR-equalizer.git'
#url_poster: '#'
#url_project: ''
#url_slides: ''
#url_source: '#'
#url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Room Impulse Response Calibration'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
#- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: example
---

### Method

Mostly referred to [Balázs Bank, 2008](https://ieeexplore.ieee.org/document/4529229)

### Dataset

Open-source Room Impulse Response from [openairlib.net](http://www.openairlib.net/auralizationdb/content/live-room-sound-studio-laboratory-university-athens) (Unfortunately, this amazing website is currently down due to unknown reasons.). The file `r8-omni-conf_b.wav` in the [GitHub repo](https://github.com/Mu-Y/RoomIR-equalizer.git) is one of the recorded Room Impulse Response wav files from a sound studio of the Laboratory of Music Acoustics Technology (LabMAT) at the Department of Music Studies of the University of Athens.

### Results (Audio Samples)

Listen to the audio samples below!

[Audio samples html page](https://mu-y.github.io/speech_samples/roomIR/)
