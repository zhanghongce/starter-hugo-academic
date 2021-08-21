---
title: "Verification of Recurrent Neural Networks for
Cognitive Tasks via Reachability Analysis"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Maxwell Shinn
- Aarti Gupta
- Arie Gurfinkel
- Nham Le
- Nina Narodytska

# Author notes (optional)

# Schedule page publish date (NOT publication's date).
publishDate: "2020-08-29T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In European Conference on Artificial Intelligence
publication_short: In ECAI

abstract: 

# Summary. An optional shortened abstract.
summary: Neural Network Verification

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

Recurrent Neural Networks (RNNs) are one of the most
successful neural network architectures that deal with temporal sequences, e.g., speech and text recognition. Recently, RNNs have been shown to be useful in cognitive neuroscience as a model of decision-making. RNNs can be trained to solve the same behavioral tasks performed by humans and other animals in decision-making experiments, allowing for a direct comparison between networks and experimental subjects. Analysis of RNNs is expected to be a simpler problem than the analysis of neural activity. However, in practice, reasoning about an RNN’s behaviour is a challenging problem. In this work, we take an approach based on formal verification for the analysis of RNNs. We make two main contributions. First, we consider the cognitive domain and formally define a set of useful properties to analyze for a popular experimental task. Second, we employ and adapt well-known verification techniques for reachability analysis to our focus domain, i.e., polytope propagation, invariant detection, and counterexample-guided abstraction refinement. Our experiments show that our techniques can effectively solve classes of benchmark problems that are challenging for state-of-the-art verification tools.