---
layout: default
---

## DistillSeq 

## Abstract

Large Language Models (LLMs) have showcased their remarkable capabilities in diverse domains, encompassing natural language understanding, translation, and even code generation. The potential for LLMs to generate harmful content is a significant concern. This risk necessitates rigorous testing and comprehensive evaluation of LLMs to ensure safe and responsible use. However, extensive testing of LLMs requires substantial computational resources, making it an expensive endeavor. Therefore, exploring cost-saving strategies during the testing phase is crucial to balance the need for thorough evaluation with the constraints of resource availability. To address this, our approach begins by transferring the moderation knowledge from an LLM to a small model. Subsequently, we deploy two distinct strategies for generating malicious queries: one based on a syntax tree approach, and the other leveraging an LLM-based method. Finally, our approach incorporates a sequential filter-test process designed to identify test cases that are prone to eliciting toxic responses. By doing so, we significantly curtail unnecessary or unproductive interactions with LLMs, thereby streamlining the testing process. Our research evaluated the efficacy of DistillSeq across four LLMs: GPT-3.5, GPT-4.0, Vicuna-13B, and Llama-13B. In the absence of DistillSeq, the observed attack success rates on these LLMs stood at 31.5% for GPT-3.5, 21.4% for GPT-4.0, 28.3% for Vicuna-13B, and 30.9% for Llama-13B. However, upon the application of DistillSeq, these success rates notably increased to 58.5%, 50.7%, 52.5%, and 54.4%, respectively. This translated to an average escalation in attack success rate by a factor of 93.0% when compared to scenarios without the use of DistillSeq. Such findings highlight the significant enhancement DistillSeq offers in terms of reducing the time and resource investment required for effectively testing LLMs.

![pipeline](/pipeline.png)



## Research Paper

**[[ISSTA 2024](https://2024.issta.org/track/issta-2024-papers#event-overview)] DistillSeq: A Framework for Safety Alignment Testing in Large Language Models using Knowledge Distillation**

*Mingke Yang, Yuqi Chen, Yi Liu, Ling Shi*

[[Preprint](https://arxiv.org/abs/2407.10106)] [[Code](https://github.com/DistillSeq/DistillSeq)]

BibTex for citation:

```
@inproceedings{yang2024distillseq,
  title={DistillSeq: A Framework for Safety Alignment Testing in Large Language Models using Knowledge Distillation},
  author={Yang, Mingke and Chen, Yuqi and Liu, Yi and Shi, Ling},
  booktitle={Proceedings of the 33rd ACM SIGSOFT International Symposium on Software Testing and Analysis},
  pages={578--589},
  year={2024}
}
```

