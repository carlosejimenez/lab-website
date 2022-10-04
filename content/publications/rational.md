---
title: "Can Rationalization Improve Robustness?"
date: 2022-04-25
draft: false
post_type: publication
authors: [hc22, jaquelinehe, karthikn, danqic]
venue: NAACL 2022
tags: []
# direct_link: https://princeton-nlp.github.io/DataMUX/

code: https://github.com/princeton-nlp/semsup
link: https://arxiv.org/abs/2202.13100
site: https://sites.google.com/princeton.edu/semantic-supervision/
---
A growing line of work has investigated the development of neural NLP models that can produce rationales–subsets of input that can explain their model predictions. In this paper, we ask whether such rationale models can also provide robustness to adversarial attacks in addition to their interpretable nature. Since these models need to first generate rationales ("rationalizer") before making predictions ("predictor"), they have the potential to ignore noise or adversarially added text by simply masking it out of the generated rationale. To this end, we systematically generate various types of ’AddText’ attacks for both token and sentence-level rationalization tasks, and perform an extensive empirical evaluation of state-of-the-art rationale models across five different tasks. Our experiments reveal that the rationale models show the promise to improve robustness, while they struggle in certain scenarios–when the rationalizer is sensitive to positional bias or lexical choices of attack text. Further, leveraging human rationale as supervision does not always translate to better performance. Our study is a first step towards exploring the interplay between interpretability and robustness in the rationalize-then-predict framework.
