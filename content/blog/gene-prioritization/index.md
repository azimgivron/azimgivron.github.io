---
title: Gene Prioritization
summary: How to discover disease causing genes ?
date: 2023-09-24

# Featured image
image:
  caption: "Gene Prioritization Package Logo"

authors:
  - admin

tags:
  - Gene Prioritization
  - Genomics
  - Matrix Completion
  - Non-Euclidean Gradient
  - Relative Smoothness

# content_meta:
#   trending: true
---

{{< toc mobile_only=true is_open=true >}}

# Gene Prioritization

In this article, I would like to discuss the problem of gene prioritization in bioinformatics. This topic was actually the subject of my master’s thesis during my second master’s degree. My goal here is to introduce the problem and discuss the biological foundations and data sources involved. We will focus first on the biological aspect, leaving the machine learning perspective for later.

Let’s talk about this task and why it even exists. To understand it, let’s recall some high school biology, particularly genetics. Living organisms are made of cells — the smallest structural and functional units of life, capable of performing all essential biological processes. Each cell is enclosed by a membrane and contains a nucleus. Between the membrane and the nucleus lies the cytoplasm, which holds various organelles — specialized structures that perform distinct functions such as energy production, protein synthesis, and waste processing.

The nucleus contains the organism’s genetic material, organized into Deoxyribonucleic Acid (DNA). DNA stores the instructions required for the organism’s development, functioning, and reproduction. It is composed of sequences of nucleotides, each consisting of a phosphate group, a deoxyribose sugar, and one of four nitrogenous bases: adenine (A), thymine (T), cytosine (C), or guanine (G). These sequences encode the information used to synthesize proteins, which perform most cellular functions — catalyzing biochemical reactions, providing structural support, transporting molecules, and regulating gene expression.

DNA is organized into chromosomes, and genes are specific segments of DNA that contain the instructions for producing particular proteins.

When we are born, all our genetic information is contained in our DNA, which holds the complete set of instructions determining how our body is formed and functions at birth. However, the environment also influences our body over time, shaping its development, physiology, and overall health. In this context, we focus on genetic alterations that disrupt normal biological regulation. Specifically, we study diseases caused by amino acid mutations, regardless of their origin, when such mutations lead to molecular dysfunctions that ultimately result in disease. Even a single amino acid substitution can alter a protein’s structure or function, impairing essential cellular processes and disturbing the delicate balance necessary for healthy physiological activity.

This is where gene prioritization becomes relevant. When studying complex diseases, thousands of genes may be potentially involved, but only a subset is truly responsible for the observed dysfunctions. Gene prioritization aims to identify and rank candidate genes that are most likely to be implicated in a specific disease. Achieving this requires integrating information from various biological data sources.

In the next sections, we will explore these data sources in more detail and discuss how they provide complementary insights into the genetic mechanisms underlying disease.
