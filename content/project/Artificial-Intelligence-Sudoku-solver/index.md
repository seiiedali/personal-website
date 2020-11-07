---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Artificial Intelligence Sudoku Solver"
summary: "Design and implement simple search, Genetic Algorithm, Simulated Annealing to solve Sudoku table using C#."
authors: [Ali Miramirkhani]
tags: ["Artificial Intelligence"]
categories: ["Artificial Intelligence"]
date: 2020-11-07T15:26:16+03:30

# Optional external URL for project (replaces project detail page).
external_link: "https://github.com/seiiedali/sudoku-solver-with-genetic-algorithm"

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
# Sudoku Solver with AI algorithms

 Solving 3\*3 and 9\*9 Sudoku table using:
- Simple search
- Simulated annealing
- Genetic algorithm

All methods and algorithm are created from scratch without the help of any pre-built module. This program is coded in C# and is developed with MS visual studio.

Procedure start from the `./Properties/Program.cs` and it will test following algorithms to solve sudoku table:
- `FourSimple.cs` which would try to solve the 4\*4 sudoku table by testing all the possible arrangement of the numbers
- `FourSA.cs` which would try to solve 4\*4 table using simulated annealing algorithm
- `FourGa` which would try to solve 4\*4 table using genetic algorithm
- `NineSimple.cs` which would try to solve the 9\*9 sudoku table by testing all the possible arrangement of the numbers
- `NineSA.cs` which would try to solve 9\*9 table using simulated annealing algorithm
- `NineGA` which would try to solve 9\*9 table using genetic algorithm
> Note that this program does not solve the table with pre entered numbers in the table but try to find the first possible arrangement of numbers into the empty table that satisfy the sudoku rules.