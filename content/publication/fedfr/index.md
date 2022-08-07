---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Federated Unsupervised Domain Adaptation for Face Recognition"
authors: 
- admin
- Xin Gan
- Xuesen Zhang
- Yonggang Wen
- Shuai Zhang
- Shuai Yi

date: 2021-05-09T09:02:27+08:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2022-03-09T09:02:27+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "IEEE International Conference on Multimedia and Expo, 2022 (ICME, Oral)"
publication_short: "ICME"

abstract: "Given labeled data in a source domain, unsupervised domain adaptation has been widely adopted to generalize models for unlabeled data in a target domain, whose data distributions are different. However, existing works are inapplicable to face recognition under privacy constraints because they require sharing of sensitive face images between domains. To address this problem, we propose federated unsupervised domain adaptation for face recognition, FedFR. FedFR jointly optimizes clustering-based domain adaptation and federated learning to elevate performance on the target domain. Specifically, for unlabeled data in the target domain, we enhance a clustering algorithm with distance constrain to improve the quality of predicted pseudo labels. Besides, we propose a new domain constraint loss (DCL) to regularize source domain training in federated learning. Extensive experiments on a newly constructed benchmark demonstrate that FedFR outperforms the baseline and classic methods on the target domain by 3% to 14% on different evaluation metrics."

# Summary. An optional shortened abstract.
summary: "We propose federated unsupervised domain adaptation for face recognition, FedFR. FedFR jointly optimizes clustering-based domain adaptation and federated learning to elevate performance on the target domain. Specifically, for unlabeled data in the target domain, we enhance a clustering algorithm with distance constrain to improve the quality of predicted pseudo labels. Besides, we propose a new domain constraint loss (DCL) to regularize source domain training in federated learning."

tags: ["federated learning", "face recognition", "unsupervised domain adaptation"]
categories: ["federated learning", "computer vision"]
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: "https://arxiv.org/abs/2105.07606"
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
projects: [fedcv]

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
