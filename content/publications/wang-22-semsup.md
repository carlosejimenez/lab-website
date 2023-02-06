---
title: "Semantic Supervision"
date: 2022-08-26
draft: false
post_type: publication
authors: [hjwang, asd, karthikn]
venue: ArXiv preprint
tags: []

code: https://github.com/princeton-nlp/semsup
link: https://arxiv.org/abs/2202.13100
site: https://sites.google.com/princeton.edu/semantic-supervision/
image: https://user-images.githubusercontent.com/8196527/200193827-9f1fb40b-35f3-4e6b-a685-0005319b6bbc.gif
---
In this paper, we propose Semantic Supervision (SemSup) - a unified paradigm for training classifiers that generalize over output spaces. In contrast to standard classification, which treats classes as discrete symbols, SemSup represents them as dense vector features obtained from descriptions of classes (e.g., "The cat is a small carnivorous mammal"). This allows the output space to be unbounded (in the space of descriptions) and enables models to generalize both over unseen inputs and unseen outputs (e.g. "The aardvark is a nocturnal burrowing mammal with long ears"). Specifically, SemSup enables four types of generalization, to – (1) unseen class descriptions, (2) unseen classes, (3) unseen super-classes, and (4) unseen tasks. Through experiments on four classification datasets across two variants (multi-class and multi-label), two input modalities (text and images), and two output description modalities (text and JSON), we show that our SemSup models significantly outperform standard supervised models and existing models that leverage word embeddings over class names. For instance, our model outperforms baselines by 40% and 20% precision points on unseen descriptions and classes, respectively, on a news categorization dataset (RCV1). SemSup can serve as a pathway for scaling neural models to large unbounded output spaces and enabling better generalization and model reuse for unseen tasks and domains.
