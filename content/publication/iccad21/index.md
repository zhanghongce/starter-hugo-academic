---
title: "Generating Architecture-Level Abstractions from RTL Designs for Processors and Accelerators Part I: Determining Architectural State Variables"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Yu Zeng
- Bo-Yuan Huang
- admin
- Aarti Gupta
- Sharad Malik

# Author notes (optional)

# Schedule page publish date (NOT publication's date).
publishDate: "2021-11-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In International Conference on Computer-Aided Design
publication_short: In ICCAD

abstract: 

# Summary. An optional shortened abstract.
summary: Constructing Instruction-Level Abstraction from RTL

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

Today's Systems-on-Chips (SoCs) comprise general/special purpose programmable processors and specialized hardware modules referred to as accelerators. These accelerators serve as co-processors and are invoked through software or firmware. Thus, verifying SoCs requires co-verification of hardware with software/firmware. Co-verification using cycle-accurate hardware models is often not scalable, and requires hardware abstractions. Among various abstractions, architecture-level abstractions are very effective as they retain only the software visible state. An Instruction-Set Architecture (ISA) serves this role for processors and such ISA-like abstractions are also desirable for accelerators. Manually creating such abstractions for accelerators is tedious and error-prone, and there is a growing need for automation in deriving them from existing Register-Transfer Level (RTL) implementations. An important part of this automation is determining which state variables to retain in the abstract model. For processors and accelerators, this set of variables is naturally the Architectural State Variables (ASVs) - variables that are persistent across instructions. This paper presents the first work to automatically determine ASVs of processors and accelerators from their RTL implementations. We propose three novel algorithms based on different characteristics of ASVs. Each algorithm provides a sound abstraction, i.e., an over-approximate set of ASVs. The quality of the abstraction is measured by the size of the set of ASVs computed. Experiments on several processors and accelerators demonstrate that these algorithms perform best in different cases, and by combining them a high quality set of ASVs can be found in reasonable time.