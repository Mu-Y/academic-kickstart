---
title: "Mis-pronunciation Detection based on Phoneme Recognition"
authors: 
  - admin
date: "2021-07-05"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: ""

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
#publication_types: ["4"]

# Publication name and optional abbreviated publication name.
publication: Project
publication_short:

abstract: "A Mis-pronunciation Detection (MPD) system. Mainly implemented the ICASSP 2020 paper [SED-MDD: Towards Sentence Dependent End-To-End Mispronunciation Detection and Diagnosis](https://ieeexplore.ieee.org/document/9052975). Some modifications are applied to improve the MPD performance. Moreover, I added an alignment module to obtain word-level alignment between the canonical phonemes (what the speaker *should* say) and the perceived phonemes (what the system recognized). Take a look at the [audio demo](https://mu-y.github.io/speech_samples/mpd_l2arctic/l2arctic_chinese.html)."

# Summary. An optional shortened abstract.
summary: "A Mis-pronunciation Detection system, with word-level aligned phonemes predictions."

tags:
- proj
featured: true

links:
- name: Audio Samples
  url: "https://mu-y.github.io/speech_samples/mpd_l2arctic/l2arctic_chinese.html"
# url_pdf: 'https://github.com/Mu-Y/SynthSing/blob/master/Final_report.pdf'
# url_code: 'https://github.com/Mu-Y/SynthSing'
# url_dataset: 'https://drive.google.com/open?id=1LQgP49jjZTb4FVEf5PevsoiBDhCIyaWp'
#url_poster: '#'
#url_project: ''
#url_slides: ''
#url_source: '#'
#url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Word-level MPD'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
#projects:
#- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

### Method

I implemented the system in the [SED-MDD paper](https://ieeexplore.ieee.org/document/9052975). Architecture is shown below.

![sed-mdd](sed-mdd.png)

Modifications: The original SED-MDD system performs frame-wise phoneme prediction, in a fashion similar to an acoustic model. However I found that the predicted phonemes were quite noisy and could not match the results reported in the paper. Here I'm using a **CTC** loss to replace the original sequence labeling module. Also, I replace the Mel input representations with [Wav2vec 2.0](https://arxiv.org/abs/2006.11477) representations. The Wav2vec 2.0 representations were extracted from a model which was unsupervisedly pre-trained on Librispeech and fine-tuned on the full 960 hours Librispeech audio.


### Dataset

I use [TIMIT](https://github.com/philipperemy/timit) and [L2-ARCTIC](https://psi.engr.tamu.edu/l2-arctic-corpus/), following the train/test split in SED-MDD.

### Results (Audio Samples)

Take a look at the audio samples below!

[Audio samples html page](https://mu-y.github.io/speech_samples/mpd_l2arctic/l2arctic_chinese.html)

### Acknowledgement

This project is a collaboration with [Shaojin Ding](https://psi.engr.tamu.edu/people/shaojin-ding/). The code was adapted from Shaojin Ding's initial implementation.

