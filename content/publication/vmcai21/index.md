---
title: "Syntax-Guided Synthesis for Lemma Generation in Hardware Model Checking"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Aarti Gupta
- Sharad Malik

# Author notes (optional)

# Schedule page publish date (NOT publication's date).
publishDate: "2021-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In Verification, Model Checking, and Abstract Interpretation
publication_short: In VMCAI

abstract: 

# Summary. An optional shortened abstract.
summary: Hardware Model Checking

tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 

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


Hardware model checking is moving from bit-level to word-level problems, 
and it is expected that model checkers can benefit when such high-level information is available.
However, for bit-vectors, it is challenging to find a good word-level interpolation strategy
for lemma generation, which hinders the use of word-level IC3/PDR algorithms.
In this work we propose to use Syntax-Guided Synthesis (SyGuS) for lemma generation in
a word-level IC3/PDR framework for bit-vector problems.