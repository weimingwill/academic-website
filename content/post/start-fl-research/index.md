---
title: "How to Kick Start Your Federated Learning Research?"
subtitle:

# Summary for listings and search engines
summary: Practical route to learn FL and conduct FL research.

# Link this post with a project
projects: []

# Date published
date: "2022-08-07T00:00:00Z"

# Date updated
lastmod: "2022-08-07T00:00:00Z"

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

Federated learning (FL) is an emerging research field that attracts considerable attention from both academia and the industry. This concept is first proposed by Google in 2016. Google aims to implement FL to Google Keyboard to protect users’ data privacy. I have been doing research on FL for several years and my Ph.D. thesis focuses on this topic. During these years, I have seen an [increasing number of top-tier publications](https://github.com/weimingwill/awesome-federated-learning/blob/master/conferences.md) and increasing adoption of this technology in companies. I would like to summarize some of my experiences and provide a three-stage route for students/researchers who want to enter this field.

This post would be useful for you if you are

- a postgraduate, who wants to conduct research in FL
- a researcher, who wants to research on FL or adopt FL to the company
- an undergraduate, who wants to focus on FL as your final year project

This post divides the process to learn FL and conduct research on FL into three different stages. In each stage, I have provided some materials that could best facilitate you and the questions you could think about while going through these materials. By the end of each stage, you would have a deeper understanding of FL.

## Stage 1: Understand Federated Learning

The objective of this stage is to understand federated learning and the challenges in FL research.

### Understand What is Federated Learning

> Estimated time to complete: is 30 mins - 1 hour

The first step is to understand the concept of federated learning (FL). Think about these questions while reading/watching the following contents:

- What is FL? How is it different from traditional machine learning?
- What are the potential applications of FL?
- What are the different categories of FL?
- Can you come up with some analogies for FL?

The following are the contents to learn from:

- [**Federated Learning Comic**](https://federated.withgoogle.com/)
- [**Federated Learning Tutorial**](https://sites.google.com/view/fl-tutorial/)
    - The whole tutorial contains a [video recording](https://slideslive.com/38935813/federated-learning-tutorial) and a [slide](https://drive.google.com/file/d/1QGY2Zytp9XRSu95fX2lCld8DwfEdcHCG/view) that introduce the FL, different types of FL, and some challenges/solutions in FL.
    - At this stage, you just need to watch the _first 20mins_.
- [Advances and Open Problems in Federated Learning](https://arxiv.org/abs/1912.04977)
    - At this stage, you just need to read the _Introduction_ of the paper (Section 1)

### Understand Challenges in Federated Learning

> Estimated time to complete: ~ 24 hours

The next step is to understand the challenges in FL if you want to conduct research in this area or adopt FL for other applications. Think about the following questions while reading the content:

- What are the challenges in FL?
- Why is it important to solve these challenges?
- Are these challenges common in all applications?
- Are these challenges equally important in applications?
- If you have a specific application in mind, you can use it as an example to analyze the potential challenges.

> Note: You may skip the solutions for these challenges at this stage.

The following are contents to learn from:

- [Federated Learning: Challenges, Methods, and Future Directions](https://arxiv.org/abs/1908.07873)
- [Federated Machine Learning: Concept and Applications](https://dl.acm.org/citation.cfm?id=3298981)
- [Federated Learning Tutorial](https://sites.google.com/view/fl-tutorial/) (Optional)
    - Although it covers challenges and some solutions of FL, the content tends to be quite technical after the first 20mins. You can skip it if you do not want to involve too many technical details and formulation at this stage.
- [Towards Federated Learning at Scale: System Design](https://arxiv.org/abs/1902.01046)
    - It covers the FL System design by Google and provides some insights into practical problems/challenges in FL systems.
- [Advances and Open Problems in Federated Learning](https://arxiv.org/abs/1912.04977)
    - Comprehensive summarization of problems and challenges in FL with a review of existing solutions.

The challenges introduced in these papers may not cover **all** important challenges (e.g., how to conduct FL without data labels), but they should be able to provide good starting points.

## Stage 2: Determine Your Focus

After understanding FL and the challenges in FL research, you will need to determine the problem you want to solve and the direction you want to continue.

### Determine the Direction

You can either choose to work on challenges you learned previously or propose a new challenge that has not been explored before. Thinking about the following questions may help you decide the problem you want to solve:

- About the problem:
    - Who else is working on the problem?
    - What will happen if you solve this problem? Will anything change in the way people do things?
    - What are the existing solutions?
- About you:
    - How relevant is the problem to you?
        - Do you experience the problem firsthand?
        - Is the problem in line with your previous research direction, your group’s research direction, or the company’s problem?
        - Are you personally interested in solving this problem?
    - Do you have advantages in solving the problem?
        - For example, if you have more experience with systems, it may be better to focus on the FL system and system heterogeneity problems.
    - Is there a meaningful milestone you can reach fast?
        - This is important as we do not want to put in effort for 2-3 years without any outcomes. It is important to break down a big problem into smaller problems.

To answer some of these questions, you may need to understand more about existing solutions to make the decision.

### Understand Existing Solutions and Analyze Gaps

You may have some challenges you want to work on in mind by now. Understanding existing solutions and analyzing the gaps could further help you make the decision. Thinking about the following questions would be beneficial when studying the existing solutions:

- What is the method and how good is it? Can you do it much better?
- What are the assumptions made in these solutions? Can you relax some of the assumptions?
- Are the datasets and source codes available for reproducing the results?
- What could be the alternative methods that can achieve better results?

You can read the solutions and details in two of the previous papers and extend your reading to more relevant papers in the field.

- [Federated Learning: Challenges, Methods, and Future Directions](https://arxiv.org/abs/1908.07873)
- [Advances and Open Problems in Federated Learning](https://arxiv.org/abs/1912.04977)
- [Papers for different FL challenges](https://github.com/weimingwill/awesome-federated-learning#paper-by-research-area)

Hopefully, this process could help you determine a direction you want to put more effort in.

## Stage 3: Start Experiments

The next step is to run experiments on the baseline solutions and implement your ideas. You can implement FL from scratch, but a better way is to use an established federated learning framework.

I would like to recommend [EasyFL](https://github.com/EasyFL-AI/easyfl), an easy-to-use federated learning platform that aims to enable users with various levels of expertise to experiment and prototype FL applications with little/no coding.

We develop EasyFL based on our years of research in this field (8 papers accepted in top-tier conferences/journals). Several of our papers in top-tier conferences (e.g., ICLR, ICCV) are developed based on it. It is simple to install and easy to use. You can run and play around with it simply on your laptop.

The following are some of the useful links:

- Github: https://github.com/EasyFL-AI/easyfl
- Tutorials: [https://easyfl.readthedocs.io/en/latest/tutorials/high-level_apis.html](https://easyfl.readthedocs.io/en/latest/tutorials/high-level_apis.html)

In this post, I have shared a route in three stages to kick-start research on federated learning. I hope that these materials could help you and smooth the learning process.

Lastly, you are encouraged to try out [EasyFL](https://github.com/EasyFL-AI/easyfl); If you find it useful, please help us star the repository and let others know.
