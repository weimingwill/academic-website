---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Optimizing Federated Unsupervised Person Re-identification via Camera-aware Clustering"
authors: 
- Jiabei Liu
- admin
- Yonggang Wen
- Jun Huang
- Wei Lin

date: 2022-09-26T01:39:02+08:00
doi: "10.1109/MMSP55362.2022.9949249"

# Schedule page publish date (NOT publication's date).
publishDate: 2022-09-26T01:39:02+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "2022 IEEE 24th International Workshop on Multimedia Signal Processing (MMSP'22)"
publication_short: "MMSP"

abstract: "Person re-identification (ReID) is a critical computer vision problem which identifies individuals from non-overlapping cameras. Many recent works on person ReID achieve remarkable performance by extracting features from large amounts of data using deep neural networks. However, the growing awareness of privacy concerns limits the development of person ReID. Prior studies employ federated person ReID to learn from decentralized edges without sharing raw data, but they overlook the variation of identities in different camera views. Concerning this issue, we propose a federated unsupervised person ReID (FedUCA) that leverages camera information to improve learning from decentralized unlabeled data. Specifically, FedUCA jointly learns person ReID models by transmitting training updates instead of raw data. We generate pseudo-labels for unlabeled local datasets on edges by clustering them into multiple groups according to different cameras. We then introduce contrastive learning with an intra-camera loss and an inter-camera loss to enhance the discrimination ability. In extensive experiments on eight person ReID datasets, our proposed approach significantly outperforms the state-of-the-art federated learning based method. It improves performance by 6% to 32% on these datasets, and notably by over 25 % on large datasets. We hope this paper will shed light on optimizing federated learning across a broader range of multimedia applications."

# Summary. An optional shortened abstract.
summary: "Person re-identification (ReID) is a critical computer vision problem which identifies individuals from non-overlapping cameras. Many recent works on person ReID achieve remarkable performance by extracting features from large amounts of data using deep neural networks. However, the growing awareness of privacy concerns limits the development of person ReID. Prior studies employ federated person ReID to learn from decentralized edges without sharing raw data, but they overlook the variation of identities in different camera views. Concerning this issue, we propose a federated unsupervised person ReID (FedUCA) that leverages camera information to improve learning from decentralized unlabeled data. Specifically, FedUCA jointly learns person ReID models by transmitting training updates instead of raw data. We generate pseudo-labels for unlabeled local datasets on edges by clustering them into multiple groups according to different cameras. We then introduce contrastive learning with an intra-camera loss and an inter-camera loss to enhance the discrimination ability. In extensive experiments on eight person ReID datasets, our proposed approach significantly outperforms the state-of-the-art federated learning based method. It improves performance by 6% to 32% on these datasets, and notably by over 25 % on large datasets. We hope this paper will shed light on optimizing federated learning across a broader range of multimedia applications."

tags: ["federated learning", "person re-identification", "computer vision"]
categories: ["federated learning", "unsupervised learning", "computer vision"]
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: https://ieeexplore.ieee.org/abstract/document/9949249
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
projects: [fedcv, fedssl]

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
