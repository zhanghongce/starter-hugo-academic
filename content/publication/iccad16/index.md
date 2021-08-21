---
title: "A Hardware-based Technique for Efficient Implicit
Information Flow Tracking"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Jangseop, Shin
- admin
- Jinyong Lee
- Ingoo Heo
- Yu-Yuan Chen
- Ruby Lee
- Yunheung Paek

# Author notes (optional)

# Schedule page publish date (NOT publication's date).
publishDate: "2016-11-01T00:00:00Z"

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
summary: Hardware information-flow tracking

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

To access sensitive information, some recent advanced attacks have been successful in exploiting implicit flows in a program in which sensitive data affects the control path and in turn affects other data. To track the sensitive data through implicit flows, several software- and hardware-based approaches have been proposed, but they suffer from the non-negligible performance overhead. In this paper, we propose a hardware tracking engine for implicit flow, called the implicit flow tracking unit (IFTU). By adopting the tracking scheme for implicit flow and mapping it to the specialized hardware, our solution can efficiently perform the implicit flow tracking with reasonable area costs.