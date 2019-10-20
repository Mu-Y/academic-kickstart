---
title: "Auto-Encoder-based Audio Denoiser"
authors: ["**Mu Yang**"]
date: "2018-10-05"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: ""

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
#publication_types: ["4"]

# Publication name and optional abbreviated publication name.
publication: "*USC course EE599: Deep Learning Lab for Speech Processing*"
publication_short:

abstract: "This assignment implements an Auto-Encoder Neural Network based Audio Denoiser. Training speech is a female speech and training noise is from cafeteria noise, while test speech is a male speech and test noise is from raining noise. The Auto-Encoder trys to reconstruct the clean audio from the mixed audio. Mel-frequency Spectrum features are used to train the Neural Network."

# Summary. An optional shortened abstract.
summary: "An Auto-Encoder Neural Network based Audio Denoiser. It trys to reconstruct the clean audio from the noise-mixed audio. Mel-frequency Spectrum features are used to train the Neural Network."

tags:
- proj
featured: true

links:
- name: Audio Samples
  url: https://soundcloud.com/mu-yang-974011976/sets/auto-encoder-audio-denoiser
#url_pdf: ''
url_code: 'https://github.com/Mu-Y/AutoEncoder-Denoiser'
#url_poster: '#'
#url_project: ''
#url_slides: ''
#url_source: '#'
#url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Waveform'
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

Mel-frequency Spectrum features are used to train the Auto-encoder Network.

For more details, take a look at the [GitHub page](https://github.com/Mu-Y/SynthSing/blob/master/Final_report.pdf).

### Dataset

Audio downloaded from YouTube. Sox is used for audio pre-processing(e.g. downsampling and trimming)

### Results(Audio Samples)

Listen to some of the audio samples below!

- Training audio
  + [Original](https://soundcloud.com/mu-yang-974011976/s_train?in=mu-yang-974011976/sets/auto-encoder-audio-denoiser)
  + [Noise-mixed](https://soundcloud.com/mu-yang-974011976/x_train?in=mu-yang-974011976/sets/auto-encoder-audio-denoiser)
  + [De-noised](https://soundcloud.com/mu-yang-974011976/d_train?in=mu-yang-974011976/sets/auto-encoder-audio-denoiser)
- Testing audio
  + [Original](https://soundcloud.com/mu-yang-974011976/s_test?in=mu-yang-974011976/sets/auto-encoder-audio-denoiser)
  + [Noise-mixed(failed due to copyright issue)]
  + [De-noised](https://soundcloud.com/mu-yang-974011976/d_test?in=mu-yang-974011976/sets/auto-encoder-audio-denoiser)

