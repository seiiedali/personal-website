---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Machine Learing SMS text classifier"
summary: "Implement supervised text classifier to detect mobile spam text messages, deploy Decision Tree and KNN models, Naive Bayes using N-Grams feature generator, TF-IDF as feature weighting method and F1-Score for accuracy evaluation with python and scikit-learn"
authors: [Ali Miramirkhani]
tags: ["Artificial Intelligence","Machine Learning","NLP"]
categories: ["Artificial Intelligence"]
date: 2020-11-06T12:12:32+03:30

# Optional external URL for project (replaces project detail page).
external_link: "https://github.com/seiiedali/Text-classifier"

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
# Text classifier
The purpose of this program is to classify text in python progrmming language using three following methods:
- Naive Bayes classifier
- Decision Tree
- KNN
Procedure of this software consist of the below phases of word processing:
## Preprocessing
In this part, different operation like:
- tokenizing
- deleting punctuations
- removing stop words
- stemming
would be performed on the input texts.
## Feature generation
Using N-grams (Unigram, Bigram and Trigram) methodologies to produce features vactor.
## Weighting features
In order to weigh feature we implement TF-IDF concepts which make it easier for accurate classification in further processing. 
## Evaluating the results
In the final stage the software would evaluate classifier using N-Gram model and result for three important criterion would be calculated which are:
- Precision
- Recall
- F1-Score