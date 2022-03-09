---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Joint Optimization in Edge-Cloud Continuum for Federated Unsupervised Person Re-identification"
authors: ["Weiming Zhuang", "Yonggang Wen", "Shuai Zhang"]
date: 2021-08-01T20:26:59+08:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2021-08-01T20:26:59+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "ACM Multimedia, 2021 (ACMMM)"
publication_short: "ACMMM"

abstract: "Person re-identification (ReID) aims to re-identify a person from non-overlapping camera views. Since person ReID data contains sensitive personal information, researchers have adopted federated learning, an emerging distributed training method, to mitigate the privacy leakage risks. However, existing studies rely on data labels that are laborious and time-consuming to obtain. We present FedUReID, a federated unsupervised person ReID system to learn person ReID models without any labels while preserving privacy. FedUReID enables in-situ model training on edges with unlabeled data. A cloud server aggregates models from edges instead of centralizing raw data to preserve data privacy. Moreover, to tackle the problem that edges vary in data volumes and distributions, we personalize training in edges with joint optimization of cloud and edge. Specifically, we propose personalized epoch to reassign computation throughout training, personalized clustering to iteratively predict suitable labels for unlabeled data, and personalized update to adapt the server aggregated model to each edge. Extensive experiments on eight person ReID datasets demonstrate that FedUReID not only achieves higher accuracy but also reduces computation cost by 29%. Our FedUReID system with the joint optimization will shed light on implementing federated learning to more multimedia tasks without data labels."

# Summary. An optional shortened abstract.
summary: ""

tags: []
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: "https://arxiv.org/abs/2108.06493"
url_code: "https://github.com/cap-ntu/FedReID"
url_dataset:
url_poster: "FedUReID_mm21_poster.pdf"
url_project:
url_slides:
url_source:
url_video: "https://youtu.be/ULDGD5XFYNc"

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

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
