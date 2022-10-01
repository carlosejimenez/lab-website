---
title: "WebShop"
date: 2022-07-16
draft: false
post_type: publication
authors: [shunyuy, hc22, jy1682, karthikn]
venue: Neural Information Processing Systems (NeurIPS) 2022
# direct_link: https://princeton-nlp.github.io/WebShop

code: https://github.com/princeton-nlp/WebShop
link: https://arxiv.org/abs/2207.01206
site: https://webshop-pnlp.github.io
---

Existing benchmarks for grounding language in interactive environments either lack real-world linguistic elements, or prove difficult to scale up due to substantial human involvement in the collection of data or feedback signals. To bridge this gap, we develop WebShop – a simulated e-commerce website environment with 1.18 million real-world products and 12,087 crowd-sourced text instructions. Given a text instruction specifying a product requirement, an agent needs to navigate multiple types of webpages and issue diverse actions to find, customize, and purchase an item. WebShop provides several challenges for language grounding including understanding compositional instructions, query (re-)formulation, comprehending and acting on noisy text in webpages, and performing strategic exploration. We collect over 1,600 human demonstrations for the task, and train and evaluate a diverse range of agents using reinforcement learning, imitation learning, and pre-trained image and language models. Our best model achieves a task success rate of 29%, which outperforms rule-based heuristics (9.6%) but is far lower than human expert performance (59%). We also analyze agent and human trajectories and ablate various model components to provide insights for developing future agents with stronger language understanding and decision making abilities. Finally, we show that agents trained on WebShop exhibit non-trivial sim-to-real transfer when evaluated on amazon.com, indicating the potential value of WebShop in developing practical web-based agents that can operate in the wild.
