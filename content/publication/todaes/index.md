---
title: "Instruction-Level Abstraction (ILA): A Uniform Specification for System-on-Chip (SoC) Verification"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Bo-Yuan Huang
- admin
- Pramod Subramanyan
- Yakir Vizel
- Aarti Gupta
- Sharad Malik

# Author notes (optional)

date: "2018-12-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2019-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In ACM Transactions on Design Automation of Electronic Systems
publication_short: In TODAES

abstract: 

# Summary. An optional shortened abstract.
summary: SoC Function Modeling and Refinement Checking

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


Modern Systems-on-Chip (SoC) designs are increasingly heterogeneous and contain specialized semi-programmable accelerators in addition to programmable processors. In contrast to the pre-accelerator era, when the ISA played an important role in verification by enabling a clean separation of concerns between
software and hardware, verification of these “accelerator-rich” SoCs presents new challenges. This article addresses these challenges by providing a formal specification and high-level abstraction for accelerator functional behavior. It formalizes the concept of an Instruction Level Abstraction (ILA) and shows its application in modeling and verification of accelerators.