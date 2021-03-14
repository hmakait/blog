---
title: "Rethinking Message Brokers on RDMA and NVM"
authors:
- admin
date: "2020-06-19"
doi: "10.1145/3318464.3384403"

# Schedule page publish date (NOT publication's date).
publishDate: "2020-06-19"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of the 2020 ACM SIGMOD International Conference on Management of Data*
publication_short: In *SIGMOD '20*

abstract: >-
  Over the last years, message brokers have become an important part of enterprise systems. 
  As microservice architectures become more popular and the need to analyze data produced by the individual services grows, companies increasingly rely on message brokers to orchestrate the flow of events between different applications as well as between data-producing services and stream processing engines that analyze the data in real-time. 
  Current state-of-the-art message brokers such as Apache Kafka or Apache Pulsar were designed for slow networks and disk-based storage. 
  In this work, we propose a new architecture that leverages remote direct memory access (RDMA) and non-volatile memory (NVM) to improve the weaknesses of existing message brokers and further scale these systems.

tags:
- message broker
- distributed
- messaging
- modern hardware
- NVRAM
- RDMA
featured: true

links:
url_pdf: 'publication/rethinking/makait_rethinking_sigmod_2020.pdf'
url_code: ''
url_dataset: ''
url_poster: 'publication/rethinking/makait_rethinking_sigmod_2020_poster.pdf'
url_project: ''
url_slides: ''
url_source: ''
url_video: 'https://www.youtube.com/watch?v=9Lpa_qOStSE'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# image:
# caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
# focal_point: ""
# preview_only: false

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
slides: example
---

