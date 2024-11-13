---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Spoken Language Intent Detection using Confusion2Vec"
authors: 
  - "Prashanth G. Shivakumar"
  - admin
  - "Panayiotis Georgiou"
author_notes:
- "Equal contribution"
- "Equal contribution"
date:  2019-09-20T16:56:26-07:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2019-09-20T16:56:26-07:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "Interspeech 2019"
publication_short: "Interspeech 2019"

abstract: "Decoding speaker’s intent is a crucial part of spoken language
understanding (SLU). The presence of noise or errors in the
text transcriptions, in real life scenarios make the task more
challenging. In this paper, we address the spoken language
intent detection under noisy conditions imposed by automatic
speech recognition (ASR) systems. We propose to employ confusion2vec word feature representation to compensate for the
errors made by ASR and to increase the robustness of the SLU
system. The confusion2vec, motivated from human speech production and perception, models acoustic relationships between
words in addition to the semantic and syntactic relations of
words in human language. We hypothesize that ASR often
makes errors relating to acoustically similar words, and the confusion2vec with inherent model of acoustic relationships between words is able to compensate for the errors. We demonstrate through experiments on the ATIS benchmark dataset, the
robustness of the proposed model to achieve state-of-the-art results under noisy ASR conditions. Our system reduces classification error rate (CER) by 20.84% and improves robustness by
37.48% (lower CER degradation) relative to the previous stateof-the-art going from clean to noisy transcripts. Improvements
are also demonstrated when training the intent detection models
on noisy transcripts."

# Summary. An optional shortened abstract.
summary: ""

tags: [paper]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: https://arxiv.org/pdf/1904.03576.pdf
url_code:
url_dataset: https://github.com/pgurunath/slu_confusion2vec
url_poster:
url_project:
url_slides:
url_source:
url_video:

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Vector Space Comparision"
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
