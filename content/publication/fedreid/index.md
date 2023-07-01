---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Performance Optimization for Federated Person Re-identification via Benchmark Analysis"
authors: 
- admin
- Yonggang Wen
- Xuesen Zhang
- Xin Gan
- Daiying Yin
- Dongzhan Zhou
- Shuai Zhang
- Shuai Yi

date: 2020-05-24T00:00:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2022-03-09T09:02:27+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "ACM Multimedia, 2020 (ACMMM, Oral)"
publication_short: ACMMM (Oral)

abstract: "Federated learning is a privacy-preserving machine learning technique that learns a shared model across decentralized clients. It can alleviate privacy concerns of personal re-identification, an important computer vision task. In this work, we implement federated learning to person re-identification (FedReID) and optimize its performance affected by statistical heterogeneity in the real-world scenario. We first construct a new benchmark to investigate the performance of FedReID. This benchmark consists of (1) nine datasets with different volumes sourced from different domains to simulate the heterogeneous situation in reality, (2) two federated scenarios, and (3) an enhanced federated algorithm for FedReID. The benchmark analysis shows that the client-edge-cloud architecture, represented by the federated-by-dataset scenario, has better performance than client-server architecture in FedReID. It also reveals the bottlenecks of FedReID under the real-world scenario, including poor performance of large datasets caused by unbalanced weights in model aggregation and challenges in convergence. Then we propose two optimization methods: (1) To address the unbalanced weight problem, we propose a new method to dynamically change the weights according to the scale of model changes in clients in each training round; (2) To facilitate convergence, we adopt knowledge distillation to refine the server model with knowledge generated from client models on a public dataset. Experiment results demonstrate that our strategies can achieve much better convergence with superior performance on all datasets. We believe that our work will inspire the community to further explore the implementation of federated learning on more computer vision tasks in real-world scenarios."

# Summary. An optional shortened abstract.
summary: "We construct a new benchmark to investigate the performance of FedReID, which contains nine datasets with different volumes sourced from different domains to simulate the heterogeneous situation in reality. The benchmark analysis reveals the bottlenecks of FedReID under the real-world scenario, including poor performance of large datasets caused by unbalanced weights in model aggregation and challenges in convergence. To address these issues, we propose two optimization methods: 1) To address the unbalanced weight problem, we propose a new method to dynamically change the weights according to the scale of model changes in clients in each training round; 2) To facilitate convergence, we adopt knowledge distillation to refine the server model with knowledge generated from client models on a public dataset."

tags: ["federated learning", "person re-identification"]
categories: ["federated learning", "computer vision"]
featured: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: https://dl.acm.org/doi/abs/10.1145/3394171.3413814
url_code: https://github.com/EasyFL-AI/EasyFL/tree/master/applications/fedreid
url_dataset:
url_poster:
url_project:
url_slides:
url_source:
url_video: https://youtu.be/LpA55fwda_g

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
