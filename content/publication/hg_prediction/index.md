---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Joint hypoglycemia prediction and glucose forecasting via deep multi-task learning"
authors: 
  - admin
  - "Darpit Dave"
  - "Madhav Erraguntla"
  - "Gerard L. Cote"
  - "Ricardo Gutierrez-Osuna"
date:  2022-05-07T16:56:26-07:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2021-10-09T16:56:26-07:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "ICASSP 2022"
publication_short: "ICASSP 2022"

abstract: 'We present a multitask learning approach to the problem of hypoglycemia (HG) prediction in diabetes.  The approach is based on a state-of-the-art time series forecasting model, N-BEATS, and extends it by adding a classification task so that the model performs both glucose forecasting (i.e., predicting future glucose values) and HG prediction (i.e., probability of future HG events sometime within the prediction horizon).  We also propose an alternative loss function that penalizes forecasting errors in the HG range.  We evaluate the approach on a dataset containing over 1.6M recordings from 112 patients with type 1 diabetes who wore a continuous glucose monitor (CGM) for 90 days.  Our results show that the classification branch significantly outperforms the forecasting branch on the problem of HG prediction, and that the new loss function is more effective at reducing forecasting errors in the HG range than multi-task learning.'

# Summary. An optional shortened abstract.
summary: ""

tags: [paper]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
#links:
#  - name: Preprint
#    url: https://arxiv.org/pdf/2110.04482.pdf
#  - name: Audio Samples
#    url: https://mu-y.github.io/speech_samples/llltts/
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: https://ieeexplore.ieee.org/document/9746129
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
