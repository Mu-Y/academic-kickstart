---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Improving Mispronunciation Detection with Wav2vec2-based Momentum Pseudo-Labeling for Accentedness and Intelligibility Assessment"
authors: ["**Mu Yang**", "Kevin Hirschi", "Stephen D. Looney", "Okim Kang", "John H. L. Hansen"]
date:  2022-05-17T16:56:26-07:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2021-10-09T16:56:26-07:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: "Interspeech 2022 (Oral)"
publication_short: "Interspeech 2022 (Oral)"

abstract: 'Current leading mispronunciation detection and diagnosis (MDD) systems achieve promising performance via end-to-end phoneme recognition. One challenge of such end-to-end solutions is the scarcity of human-annotated phonemes on natural L2 speech. In this work, we leverage unlabeled L2 speech via a pseudo-labeling (PL) procedure and extend the fine-tuning approach based on pre-trained self-supervised learning (SSL) models. Specifically, we use Wav2vec 2.0 as our SSL model, and fine-tune it using original labeled L2 speech samples plus the created pseudo-labeled L2 speech samples. Our pseudo labels are dynamic and are produced by an ensemble of the online model on-the-fly, which ensures that our model is robust to pseudo label noise. We show that fine-tuning with pseudo labels gains a 5.35% phoneme error rate reduction and  2.48% MDD F1 score improvement over a labeled-samples-only fine-tuning baseline. The proposed PL method is also shown to outperform conventional offline PL methods. Compared to the state-of-the-art MDD systems, our MDD solution achieves a more accurate and consistent phonetic error diagnosis. In addition, we conduct an open test on a separate UTD-4Accents dataset, where our system recognition outputs show a strong correlation with human perception, based on accentedness and intelligibility.'

# Summary. An optional shortened abstract.
summary: ""

tags: [paper]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
  - name: Preprint
    url: https://arxiv.org/pdf/2203.15937.pdf
  - name: Audio Samples
    url: https://mu-y.github.io/speech_samples/mdd_IS22/
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

# url_pdf: https://arxiv.org/pdf/1904.03576.pdf
# url_code:
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
