---
title: "Synthing: A WaveNet-based Singing Voice Synthisizer"
authors: 
  - admin
  - "James Bunning"
  - "Shiyu Mou"
  - "Sharada Murali"
  - "Yixin Yang"
date: "2018-12-05"
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

abstract: "Recent advances in synthesizing singing voice from a music score and lyrics have been achieved using a Neural Parametric Singing Synthesizer ([NPSS](https://www.mdpi.com/2076-3417/7/12/1313)) based on a modified version of the WaveNet architecture. This model trains on phonetic transcriptions of lyrics and acoustic features, and is able to significantly reduce training and generation times while still achieving the sound quality and naturalness of state-of-the-art concatenative systems. Although NPSS can model a specific singer’s voice and style of singing, it cannot generate a new singing performance given new singer data. SynthSing, our WaveNet-based singing synthesizer, expands on the NPSS synthesizer to generate a singer’s voice given new singing data and has the potential to transform the timbre of one singer’s voice into that of another singer. We found that the WaveNet-based model produces superior results in terms of naturalness and sound quality."

# Summary. An optional shortened abstract.
summary: "Final project for USC course EE599: Deep Learning Lab for Speech Processing - a WaveNet-based singing voice synthesizer. This is a partial implementation of the paper [A Neural Parametric Singing Synthesizer Modeling Timbre and Expression from Natural Songs](https://www.mdpi.com/2076-3417/7/12/1313)."

tags:
- proj
featured: true

links:
- name: Audio Samples
  url: "https://mu-y.github.io/speech_samples/synthsing/"
url_pdf: 'https://github.com/Mu-Y/SynthSing/blob/master/Final_report.pdf'
url_code: 'https://github.com/Mu-Y/SynthSing'
url_dataset: 'https://drive.google.com/open?id=1LQgP49jjZTb4FVEf5PevsoiBDhCIyaWp'
#url_poster: '#'
#url_project: ''
#url_slides: ''
#url_source: '#'
#url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Timbre Model Architecture'
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

We implemented the Timbre model mentioned in the framework of the [NPSS](https://www.mdpi.com/2076-3417/7/12/1313) paper. 

Unlike the vanilla sample-to-sample WaveNet, the proposed model makes frame-to-frame predictions on 60-dimensional log-Mel Spectral Frequency Coefficients(**MFSCs**)and 4-dimensional Band Aperiodicity(**AP**) Coefficients, using F0(coarse coded), phoneme identity(one-hot coded) and normalized phoneme position(coarse coded) as local control inputs and singer identity as global control inputs. Then we feed generated MFSCs and APs, as well as true F0 into WORLD vocoder to synthesize audio. The features, i.e. MFSCs, APs and F0 are also extracted via WORLD.

For more details, take a look at our [report](https://github.com/Mu-Y/SynthSing/blob/master/Final_report.pdf) and the original [NPSS paper](https://www.mdpi.com/2076-3417/7/12/1313).

### Dataset

We used two datasets: 1) NIT Japanese Nursery dataset ([NIT-SONG070-F001](http://hts.sp.nitech.ac.jp/archives/2.3/HTSdemo_NIT-SONG070-F001.tar.bz2)) and 2) self-curated Coldplay songs dataset.

### Results (Audio Samples)

Listen to some of our sythesized audio samples below!

[Audio samples html page](https://mu-y.github.io/speech_samples/synthsing/)

