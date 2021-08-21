---
title: "ILAng: a Modeling and Verification Platform for SoCs using Instruction-Level Abstractions"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Bo-Yuan Huang
- admin
- Aarti Gupta
- Sharad Malik

# Author notes (optional)

date: "2019-04-04T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2019-04-04T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In Tools and Algorithms for the Construction and Analysis of Systems
publication_short: In TACAS

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


We present ILAng, a platform for modeling and verification
of systems-on-chip (SoCs) using Instruction-Level Abstractions (ILA).
The ILA formal model targeting the hardware-software interface enables
a clean separation of concerns between software and hardware through
a unified model for heterogeneous processors and accelerators. Top-down it provides a specification for functional verification of hardware,
and bottom-up it provides an abstraction for software/hardware co-verification. ILAng provides a programming interface for (i) constructing
ILA models (ii) synthesizing ILA models from templates using program
synthesis techniques (iii) verifying properties on ILA models (iv) behavioral equivalence checking between different ILA models, and between an
ILA specification and an implementation. It also provides for translating models and properties into various languages (e.g., Verilog and SMT
LIB2) for different verification settings and use of third-party verification tools. This paper demonstrates selected capabilities of the platform through case studies.