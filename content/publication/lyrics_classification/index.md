---
title: "Collection and Classification of Lyrics"
authors: ["**Mu Yang**", "Tao Chen", "Chang Su", "Zhe Yang"]
date: "2018-11-20"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: ""

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
#publication_types: ["4"]

# Publication name and optional abbreviated publication name.
publication: "*USC course CSCI544: Applied Natural Language Processing*"
publication_short:

abstract: "Web crawler of lyrics and corresponding music genre. Multiple baseline classifiers, including KNN, Naive Bayes, LSTM are applied to identify genre of a song by analyzing its lyrics."

# Summary. An optional shortened abstract.
summary: "Web crawler of lyrics and corresponding music genre. Multiple baseline classifiers, such as Naive Bayes, SVM and Neural Approach(LSTM) are applied to identify the genre of a song by analyzing its lyrics."

tags:
- proj
featured: true

links:
#- name: Audio Samples
 # url: https://soundcloud.com/mu-yang-974011976/sets/roomir-equalizer
url_pdf: 'https://github.com/Mu-Y/CSCI544_Prj/blob/master/final_report.pdf'
url_code: 'https://github.com/Mu-Y/CSCI544_Prj'
#url_poster: '#'
#url_project: ''
#url_slides: ''
#url_source: '#'
#url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ''
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

#### Lyrics Collection

We start from a list of artists. We utilize the [iTunes Search API](https://developer.apple.com/library/archive/documentation/AudioVideo/Conceptual/iTuneSearchAPI/index.html) to request meta data for each artist, including song name, genre, album/collection name, release year, etc. Then a web crawler is applied to fetch lyrics on [Genius](https://genius.com/), using artist names and song names. Finally the collected lyrics are cleaned up by some basic processing: removing too-short lyrics, deduplication, etc.

#### Classifiers

We applied the following classifiers to compare their performances:

- KNN, with TF-IDF as features
- Naive Bayes, with TF-IDF as features
- SVM, with TF-IDF as features
- LSTM, with Glove word embedding as features

For more details, take a look at our [report](https://github.com/Mu-Y/CSCI544_Prj/blob/master/final_report.pdf).


### Results

**Lyrics Collection:** We manage to obtain a lyrics-genre dataset, with 30649 lyrics from 8 genres.

**Classifiers:** We train the classifiers on a balanced set - 390 lyrics for each genre, from which we hold out a balanced set as test set. Accuracy on the held-out test set is presented below.

| Model         | Accuracy         
| ------------- |:-------------:
| KNN           | 0.426
| Naive Bayes   | **0.597**      
| SVM           | 0.588      
| LSTM          | 0.563        

Interestingly, the Baive Bayes Classifier works pretty well, outperforming all others. That said, I have to recognize, the LSTM model has a few hyperparameters(e.g. hidden layer dimension, learning rate, etc) to be tuned. But due to the time and computation resource limitation, these tuning are not adequately performed. It'll be interesting to see in the future that whether there will be more performance boost with a thorough parameter tuning.