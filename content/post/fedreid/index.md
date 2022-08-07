---
title: "Federated Person Re-identification: Benchmark, In-Depth Analysis, and Performance Optimization"
subtitle:  

# Summary for listings and search engines
summary: Performance optimization for federated person re-identification via benchmark analysis.

# Link this post with a project
projects: []

# Date published
date: "2020-10-05T00:00:00Z"

# Date updated
lastmod: "2020-10-05T00:00:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/CpkOjOcXdUY)'
  # focal_point: ""
  # placement: 2
  # preview_only: false

authors:
- admin

tags:
- research
- federated learning

categories:
- research
---

This paper is accepted in ACMMM'20 Oral.

>Paper: Performance Optimization for Federated Person Re-identification via Benchmark Analysis
>
>Github: https://weiming.me/publication/fedreid

Personal re-identification (ReID) is an important computer vision task, but its development is constrained by the increasing privacy concerns. Federated learning is a privacy-preserving machine learning technique that learns a shared model across decentralized clients. In this paper, we implement federated learning to person re-identification (FedReID) and optimize its performance affected by statistical heterogeneity in the real-world scenario by analyzing insights from a newly constructed benchmark.

> Statistical heterogeneity is caused by:
> 1. Non-independent and identifical distribution (non-IID) data;
> 2. Unbalanced data volume of clients

![image-20201015161300388](https://imgur.com/wGgcOPT.png)

This article aims to give a brief introduction of the paper from three points:
Benchmark, including datasets, a new federated algorithm, and scenarios
Insights of benchmark analysis
Performance optimization methods:

## Benchmark

### Datasets
The benchmark contains 9 most popular ReID datasets, whose details are as follows:

![image-20201015162805483](https://imgur.com/gihH7Ug.png)

These datasets source from different domains and vary in the number of images and identities, which simulates the statistical heterogeneity in the real-world scenario.

## Algorithm: Federated Partial Averaging

We propose a new algorithm - Federated Partial Averaging (FedPav) because the standard federated algorithm Federated Averaging (FedAvg) requires the identical model in the server and the clients. While client models are different in FedReID, because in each client, the dimension of the classifier depends on the number of ids, which is different in different datasets in clients.

![img](https://imgur.com/2kB35i5.png)

FedPav only syncs part of client models with the server. The training steps with FedPav are as followed:

1. A server sends the global model to clients.
2. Clients use local data to train the models with their classifiers, obtaining local models
3. Clients upload the backbone parameters
4. The server aggregates model updates, obtaining a new global model.

## Insights from Benchmark Analysis
We provide several insights by analyzing the benchmark results in the paper. In the article, we highlight two of them that reveal the impact of statistical heterogeneity.

### 1. Large datasets in Federated Learning achieve lower accuracy than local training

![image-20201015162703398](https://imgur.com/x04ImWW.png)

* FedPav: the performance of the global model in federated learning
* FedPav Local: the performance of the local model in clients before uploading to the server.
* Local training: baseline, the performance of training using one data set.

Local Training outperforms federated learning, which defeats the purpose for the large datasets to participate in the training.

### 2. Federated learning does not guarantee

The training accuracies of testing fluctuate through the training.

![image-20201015162716243](https://imgur.com/DlFdKn6.png)

## Performance Optimization

### Knowledge Distillation to Facilitate Convergence

![image-20201015163720421](https://imgur.com/bNGvxkI.png)
<!-- ![img](https://i.imgur.com/lpVt8Ip.png) -->

We adopt knowledge distillation to better transfer knowledge from the teachers to the student, regarding clients as teachers and the server as the student.

Knowledge distillation effectively improve the convergence of FedReID (orange line in the figure)

![image-20201015162731576](https://imgur.com/WKXbXbj.png)


### Weight Adjustment to Improve Performance

![img](https://imgur.com/nTU2VcI.png)
<!-- ![img](https://i.imgur.com/HnPpG2E.png) -->

We adjust the weights for aggregation using cosine distance weight. The intuition behind is that the clients who have larger changes should contribute more in model aggregation such that more newly learned knowledge can reflect in the aggregated model.

The local model of federated learning with cosine distance weight outperforms local training in all datasets.

![image-20201015162747403](https://imgur.com/kJuZCv4.png)

## Conclusion

This paper implements federated learning to person re-identification to mitigate the privacy concern of centralizing a large amount of image data. To optimize federated person re-identification (FedReID) under statistical heterogeneity, we construct a benchmark and conduct an in-depth analysis of the benchmark results.
Please refer to the paper and the codes for more details about the algorithms and experiments.
