---
title: "ILA-MCM: Integrating Memory Consistency Models with Instruction-Level Abstractions for Heterogeneous System-on-Chip Verification"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Caroline Trippel
- Grigory Fedyukovich
- Yatin A. Manerkar
- Aarti Gupta
- Margaret Martonosi
- Sharad Malik

# Author notes (optional)

# Schedule page publish date (NOT publication's date).
publishDate: "2018-10-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In Formal Methods in Computer-Aided Design
publication_short: In FMCAD

abstract: 

# Summary. An optional shortened abstract.
summary: Memory Consistency Model

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


Modern Systems-on-Chip (SoCs) integrate heterogeneous compute elements ranging from non-programmable specialized accelerators to programmable CPUs and GPUs. 
To ensure correct system behavior, SoC verification techniques must account for
inter-component interactions through shared memory, which necessitates reasoning about memory consistency models.
This paper presents ILA-MCM, a symbolic reasoning framework for automated SoC verification, 
where MCMs are integrated with Instruction-Level Abstractions (ILAs) that have been proposed to model architecture-level program-visible states and state updates in heterogeneous SoC components. ILA-MCM enables reasoning about system-wide properties that depend on functional state 
updates as well as ordering relations between them.