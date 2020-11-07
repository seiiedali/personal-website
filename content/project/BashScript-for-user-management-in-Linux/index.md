---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "BashScript for User Management in Linux"
summary: "Develop Linux Shell program to fully create/delete/check system users using Bash Script"
authors: [Ali Miramirkhani]
tags: ["Linux","Bash Script","Shell"]
categories: ["Linux Shell"]
date: 2020-11-07T16:00:30+03:30

# Optional external URL for project (replaces project detail page).
external_link: "https://github.com/seiiedali/BashScript-for-user-management"

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
# User Management Bash script for Linux
General bash script which would
- Create a user
- Checkout a user
- Delete the user

## Creating the user
Provided script will check for user name correctness (if it is empty or duplicate) then it create a the user with its own:
- group
- home directory
- UID and GID
then it will configure related files and save a log for this activity

## Checking out an user
Like creating the user, the script will check if the entered user is existed and available and then it return the related data about the user. This action also save a log in `/var/log/usermanagement.log`.

## Deleting the user
This part delete the user after authenticating its existence. Deleting an user includes:
- deleting home directory
- deleting email directory
- deleting records from related configuration files
    - `/etc/passwd`
    - `/etc/shadow`
    - `/etc/group`
and finally it will save a log of this action.

>A very detailed documentation of this project is provided  in `./Documentation.pdf` in Persian to check out more about this script.