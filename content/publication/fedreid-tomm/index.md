---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Optimizing Performance of Federated Person Re-identification: Benchmarking and Analysis"
authors: 
- admin
- Xin Gan
- Yonggang Wen
- Shuai Zhang
date: 2020-10-22T01:49:32+08:00
doi: "10.1145/3531013"

# Schedule page publish date (NOT publication's date).
publishDate: 2022-04-22T01:49:32+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "ACM Transactions on Multimedia Computing, Communications, and Applications (TOMM)"
publication_short: "TOMM"

abstract: "The increasingly stringent data privacy regulations limit the development of person re-identification (ReID) because person ReID training requires centralizing an enormous amount of data that contains sensitive personal information. To address this problem, we introduce federated person re-identification (FedReID) — implementing federated learning, an emerging distributed training method, to person ReID. FedReID preserves data privacy by aggregating model updates, instead of raw data, from clients to a central server. Furthermore, we optimize the performance of FedReID under statistical heterogeneity via benchmark analysis. We first construct a benchmark with an enhanced algorithm, two architectures, and nine person ReID datasets with large variances to simulate the real-world statistical heterogeneity. The benchmark results present insights and bottlenecks of FedReID under statistical heterogeneity, including challenges in convergence and poor performance on datasets with large volumes. Based on these insights, we propose three optimization approaches: (1) We adopt knowledge distillation to facilitate the convergence of FedReID by better transferring knowledge from clients to the server; (2) We introduce client clustering to improve the performance of large datasets by aggregating clients with similar data distributions; (3) We propose cosine distance weight to elevate performance by dynamically updating the weights for aggregation depending on how well models are trained in clients. Extensive experiments demonstrate that these approaches achieve satisfying convergence with much better performance on all datasets. We believe that FedReID will shed light on implementing and optimizing federated learning on more computer vision applications."

# Summary. An optional shortened abstract.
summary: "We construct a new benchmark to investigate the performance of federated person re-identification (FedReID), which contains nine datasets with different volumes sourced from different domains to simulate the heterogeneous situation in reality. The benchmark analysis reveals the bottlenecks of FedReID under the real-world scenario, including poor performance of large datasets caused by unbalanced weights in model aggregation and challenges in convergence. To address these issues, we propose three optimization methods: 1) We adopt knowledge distillation to facilitate the convergence of FedReID by better transferring knowledge from clients to the server; 2) We introduce client clustering to improve the performance of large datasets by aggregating clients with similar data distributions; 3) We propose cosine distance weight to elevate performance by dynamically updating the weights for aggregation depending on how well models are trained in clients."

tags: ["federated learning", "person re-identification"]
categories: ["federated learning", "computer vision"]
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: https://dl.acm.org/doi/10.1145/3531013
url_code: https://github.com/EasyFL-AI/EasyFL/tree/master/applications/fedreid
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
