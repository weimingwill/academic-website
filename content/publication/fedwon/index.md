---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Is Normalization Indispensable for Multi-domain Federated Learning?"
authors: 
- admin
- Lingjuan Lyu
date: 2023-06-13T10:34:53+08:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2023-06-13T10:34:53+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: "Preprint"
publication_short: ""

abstract: "Federated learning (FL) enhances data privacy with collaborative in-situ training on decentralized clients. Nevertheless, FL encounters challenges due to non-independent and identically distributed (non-i.i.d) data, leading to potential performance degradation and hindered convergence. While prior studies predominantly addressed the issue of skewed label distribution, our research addresses a crucial yet frequently overlooked problem known as multi-domain FL. In this scenario, clients' data originate from diverse domains with distinct feature distributions, as opposed to label distributions. To address the multi-domain problem in FL, we propose a novel method called Federated learning Without normalizations (FedWon). FedWon draws inspiration from the observation that batch normalization (BN) faces challenges in effectively modeling the statistics of multiple domains, while alternative normalization techniques possess their own limitations. In order to address these issues, FedWon eliminates all normalizations in FL and reparameterizes convolution layers with scaled weight standardization. Through comprehensive experimentation on four datasets and four models, our results demonstrate that FedWon surpasses both FedAvg and the current state-of-the-art method (FedBN) across all experimental setups, achieving notable improvements of over 10% in certain domains. Furthermore, FedWon is versatile for both cross-silo and cross-device FL, exhibiting strong performance even with a batch size as small as 1, thereby catering to resource-constrained devices. Additionally, FedWon effectively tackles the challenge of skewed label distribution."

# Summary. An optional shortened abstract.
summary: "We propose FedWon, a novel method that eliminates normalizations in FL and utilizes scaled weight standardization for multi-domain federated learning. Experimental results on four datasets and models show that FedWon outperforms FedAvg and the state-of-the-art method (FedBN), with improvements exceeding 10% in certain domains. FedWon is versatile for both cross-silo and cross-device FL, even with a small batch size of 1, catering to resource-constrained devices. It also effectively addresses the challenge of skewed label distribution."

tags: ["federated learning", "multi-domain fl"]
categories: ["federated learning"]
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: https://arxiv.org/abs/2306.05879
url_code: 
url_dataset: 
url_poster:
url_project:
url_slides:
url_source:
url_video:

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
projects:

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
