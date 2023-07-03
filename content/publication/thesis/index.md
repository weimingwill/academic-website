---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Toward A Generic Federated Learning Platform Optimized For Computer Vision Applications"
authors: [admin]
date: 2022-12-22T01:57:22+08:00
doi: "10.32657/10356/164712"

# Schedule page publish date (NOT publication's date).
publishDate: 2022-12-22T01:57:22+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["7"]

# Publication name and optional abbreviated publication name.
publication: "Thesis, Nanyang Technological University"
publication_short: "Thesis"

abstract: "As a result of advances in deep learning, computer vision has transformed many industries with a wide range of applications. The majority of these applications heavily rely on centralizing plenty of images to train deep neural networks. However, this centralized training approach is becoming infeasible due to the increasingly stringent data privacy regulations, especially for privacy-sensitive computer vision applications like face recognition and person re-identification that contain sensitive personal information in training images. Federated learning (FL) is an emerging distributed training paradigm that preserves data privacy via in-situ model training on decentralized data. Implementing FL to computer vision applications, however, is not optimized in terms of the performance of the system and specific computer vision applications. In this thesis, we aim to optimize the FL platform for computer vision applications via system and algorithm optimizations. Firstly, we perform system optimization of FL systems and develop the first low-code FL platform, EasyFL, to improve researchers' productivity and eﬃciency in implementing new federated computer vision applications. We achieve this goal while ensuring great flexibility for customization by unifying simple API design, modular design, and granular training flow abstraction. Our evaluation demonstrates that EasyFL allows users to write less code and our distributed training optimization effectively accelerates training speed by 1.5 times. Built on EasyFL, we optimize algorithms for the following three computer vision applications: person re-identification (ReID), unsupervised person ReID, and self-supervised learning. We propose federated person ReID (FedReID), a new paradigm of person ReID training, and investigate its performance under statistical heterogeneity via benchmark analysis. Based on the insights from these analysis, we propose three optimization methods to elevate performance: client clustering, knowledge distillation, and weight adjustment. Extensive experiments demonstrate that these approaches achieve satisfying convergence with much better performance on all datasets. We further introduce the first federated unsupervised person ReID system (FedUReID), which learns person ReID models from decentralized edges without any labels. We elevate its performance via edge-cloud joint optimization. As a result, our methods not only achieve higher accuracy but also reduce computation costs by 29%. Next, we advance self-supervised visual representation learning to learn from decentralized data by proposing the federated self-supervised learning (FedSSL) framework. Based on the framework, we conduct empirical studies to uncover in-depth insights into essential and useful fundamental building blocks in FedSSL . Inspired by these insights, we introduce a new approach to tackle the divergence issue caused by statistical heterogeneity. Extensive empirical studies demonstrate that our proposed approach is superior to existing methods in a wide range of settings. Moving forward from optimizing a single application, FL system could have multiple simultaneous training activities for multiple applications in real-world scenarios, such as autonomous vehicles. We design a smart multi-tenant FL system that effectively coordinates and executes multiple simultaneous FL training activities. We first formalize the problem of multi-tenant FL, define multi-tenant FL scenarios, and introduce a vanilla multi-tenant FL system that trains activities sequentially to form baselines. Then, we propose two approaches to optimize multi-tenant FL by considering both synergies and differences among these training activities. Extensive experiments demonstrate that our method outperforms other methods while consuming 40% less energy. We believe that our optimization approaches and insights will inspire practitioners to further explore the implementation and optimization of federated computer vision applications."

# Summary. An optional shortened abstract.
summary: ""

tags: ["federated learning", "computer vision"]
categories: ["federated learning", "computer vision"]
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: https://dr.ntu.edu.sg/handle/10356/164712
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
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
