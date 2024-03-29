---
title: "DataMUX: Data Multiplexing for Neural Networks"
date: 2022-07-16
draft: false
post_type: publication
authors: [murahari, carlosej, runzhey, karthikn]
venue: NeurIPS 2022
tags: ["Machine Learning", "Parallel Computing", "Computational Engineering"]

code: https://github.com/princeton-nlp/DataMUX
link: https://arxiv.org/abs/2202.09318
site: https://princeton-nlp.github.io/DataMUX/
image: https://princeton-nlp.github.io/DataMUX/assets/photos/teaser.gif
---
In this paper, we introduce data multiplexing (DataMUX), a technique that enables deep neural networks to process multiple inputs simultaneously using a single compact representation. DataMUX demonstrates that neural networks are capable of generating accurate predictions over mixtures of inputs, resulting in increased throughput with minimal extra memory requirements. Our approach uses two key components -- 1) a multiplexing layer that performs a fixed linear transformation to each input before combining them to create a mixed representation of the same size as a single input, which is then processed by the base network, and 2) a demultiplexing layer that converts the base network's output back into independent representations before producing predictions for each input. We show the viability of DataMUX for different architectures (Transformers, and to a lesser extent MLPs and CNNs) across six different tasks spanning sentence classification, named entity recognition and image classification. For instance, DataMUX for Transformers can multiplex up to 20x/40x inputs, achieving 11x/18x increase in throughput with minimal absolute performance drops of <2% and <4% respectively on MNLI, a natural language inference task. We also provide a theoretical construction for multiplexing in self-attention networks and analyze the effect of various design elements in DataMUX.
