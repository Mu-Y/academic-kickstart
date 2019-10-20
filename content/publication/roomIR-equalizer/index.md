---
title: "Parallel Second-order Filter-based Equalizer for Digital Room Correction"
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

abstract: "Room Acoustics matters. Producers in studio need to monitor every subtle detail in music. Every ordinary people wants excellent sound quality for their playback system to enjoy movies, music, TV broadcast, etc. However, if the room where the sound system is installed gives undesired acoustical effect on the audio, these wishes could never come true, no matter how much money you invest in your electronic playback system. Bad room acoustics is a common problem in almost every realistic room. That is why we need extra calibration technologies to make up for the acoustical effect, or to put it more specifically, the frequency response of the room.  <br /> <br /> In this project, a Parallel second-order-based equalizer design method is deployed for loudspeaker-room correction problem. "

# Summary. An optional shortened abstract.
summary: "A Parallel second-order-based equalizer for Room Impulse Response Calibration."

tags:
- proj
featured: true

links:
- name: Audio Samples
  url: https://soundcloud.com/mu-yang-974011976/sets/roomir-equalizer
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

Open-source Room Impulse Response from [openairlib.net](http://www.openairlib.net/auralizationdb/content/live-room-sound-studio-laboratory-university-athens)(Unfortunately, this amazing website is currently down due to unknown reasons.). The file `r8-omni-conf_b.wav` in the [GitHub repo](https://github.com/Mu-Y/RoomIR-equalizer.git) is one of the recorded Room Impulse Response wav files from a sound studio of the Laboratory of Music Acoustics Technology (LabMAT) at the Department of Music Studies of the University of Athens.

### Results(Audio Samples)

Convolve audio with the Room Impulse Responses, to hear the impact of Room Impulse Response on the listening experience, and also the calibration of the equalizer.

- Sound studio Impulse Response(data accompanying this repo), audio is a classical music clip.
  - Original: [audio](https://soundcloud.com/mu-yang-974011976/classic-short?in=mu-yang-974011976/sets/roomir-equalizer)
  - Conv with Room Impulse Response: [audio](https://soundcloud.com/mu-yang-974011976/classic-short-live-studio?in=mu-yang-974011976/sets/roomir-equalizer)
  - Conv with **Equalized** Room Impulse Response: [audio](https://soundcloud.com/mu-yang-974011976/classic-short-live-studio-eq?in=mu-yang-974011976/sets/roomir-equalizer)

- Another Impulse Response from an office room, audio is an EDM clip.
  - Original: [audio](https://soundcloud.com/mu-yang-974011976/edm-short?in=mu-yang-974011976/sets/roomir-equalizer)
  - Conv with Room Impulse Response: [audio](https://soundcloud.com/mu-yang-974011976/edm-short-air-office?in=mu-yang-974011976/sets/roomir-equalizer)
  - Conv with **Equalized** Room Impulse Response: [audio](https://soundcloud.com/mu-yang-974011976/edm-short-air-office-eq?in=mu-yang-974011976/sets/roomir-equalizer)