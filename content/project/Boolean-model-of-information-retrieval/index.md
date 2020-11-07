---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Boolean Model of Information Retrieval"
summary: "Design and implement Boolean Information Retrieval Model on corpus text documents for boolean and positional search queries using python"
authors: [Ali Miramirkhani]
tags: ["Semantic Web", "Information Retrieval"]
categories: ["Semantic Web"]
date: 2020-11-07T15:22:47+03:30

# Optional external URL for project (replaces project detail page).
external_link: "https://github.com/seiiedali/Boolean-model-of-information-retrieval"

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
# Boolean model of information retrieval
 This program will interpret documents, index the words into a dictionary and finally, it will be possible to search through docs with boolean method

## Documents Interpreting
In the first part of `main.py` the code will use the `GetDocText.py` module to read all the available docs and then index it. After reading the text, below tasks are operated on them:
- splitting and tokenizing the words from the text
- preprocess token (lower case + punctuations removal + excluding dirty tokens)
- indexing tokens into the dictionary (docID + tokenPosision + frequency)
## Loging activity
On each program run, a full log will be saved in `./log` with the name of `[Date + Time]` which contains below information:
- available documents
- dictionary data
- entered query and results
## Searching for query
The program will ask you to enter your desired query, which can contains up to 3 word and 2 operator
> for example: `that WITH he WITH is` is an acceptable query
allowed operator are:
- AND
- OR
- WITH
- NEAR #
which can place within the the query tokens
Finally, all possible answers (related documnets) will be shown