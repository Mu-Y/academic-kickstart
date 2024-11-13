---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "DiariST: Streaming Speech Translation with Speaker Diarization"
authors:
  - admin
  - Naoyuki Kanda
  - Xiaofei Wang
  - Junkun Chen
  - Peidong Wang
  - Jian Xue
  - Jinyu Li
  - Takuya Yoshioka

date:  2024-04-13T16:56:26-07:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2024-01-04T16:56:26-07:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "ICASSP 2024"
publication_short: 'ICASSP 2024'

abstract: 'End-to-end speech translation (ST) for conversation recordings involves several under-explored challenges such as speaker diarization (SD) without accurate word time stamps and handling of overlapping speech in a streaming fashion. In this work, we propose DiariST, the first streaming ST and SD solution. It is built upon a neural transducer-based streaming ST system and integrates token-level serialized output training and t-vector, which were originally developed for multi-talker speech recognition. Due to the absence of evaluation benchmarks in this area, we develop a new evaluation dataset, DiariST-AliMeeting, by translating the reference Chinese transcriptions of the AliMeeting corpus into English. We also propose new metrics, called speaker-agnostic BLEU and speaker-attributed BLEU, to measure the ST quality while taking SD accuracy into account. Our system achieves a strong ST and SD capability compared to offline systems based on Whisper, while performing streaming inference for overlapping speech. To facilitate the research in this new direction, we release the evaluation data, the offline baseline systems, and the evaluation code.'

# Summary. An optional shortened abstract.
summary: ""

tags: [paper]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
 - name: PDF
   url: https://arxiv.org/pdf/2309.08007.pdf
  # - name: Audio Samples
    # url: https://mu-y.github.io/speech_samples/llltts/
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

# url_pdf: https://arxiv.org/pdf/2110.04482.pdf
# url_code: https://github.com/Mu-Y/lll-tts
# url_dataset: https://github.com/pgurunath/slu_confusion2vec
# url_poster:
# url_project:
# url_slides:
# url_source:
# url_video:

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
# image:
#   caption: "Vector Space Comparision"
#   focal_point: ""
#   preview_only: false

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
