---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Learning ASR pathways: A sparse multilingual ASR model"
authors: ["**Mu Yang**", "Andros Tjandra", "Chunxi Liu", "David Zhang", "Duc Le", "John H. L. Hansen", "Ozlem Kalinli"]
date:  2022-09-13T16:56:26-07:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2022-09-13T16:56:26-07:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "Arxiv preprint, 2022"
publication_short: "Arxiv preprint, 2022"

abstract: 'Neural network pruning can be effectively applied to compress automatic speech recognition (ASR) models. However, in multilingual ASR, performing language-agnostic pruning may lead to severe performance degradation on some languages because language-agnostic pruning masks may not fit all languages and discard important language-specific parameters. In this work, we present ASR pathways, a sparse multilingual ASR model that activates language-specific sub-networks (pathways), such that the parameters for each language are learned explicitly. With the overlapping sub-networks, the shared parameters can also enable knowledge transfer for lower resource languages via joint multilingual training. We propose a novel algorithm to learn ASR pathways, and evaluate the proposed method on 4 languages with a streaming RNN-T model. Our proposed ASR pathways outperform both dense models (-5.0% average WER) and a language-agnostically pruned model (-21.4% average WER), and provide better performance on low-resource languages compared to the monolingual sparse models.'

# Summary. An optional shortened abstract.
summary: ""

tags: [paper]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
 - name: Preprint
   url: https://arxiv.org/pdf/2209.05735.pdf
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
