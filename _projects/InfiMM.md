---
layout: page
title: InfiMM
description: Advanced Flamingo reproduction
img: https://huggingface.co/Infi-MM/infimm-zephyr/resolve/main/assets/infimm-logo.webp
importance: 1
category: work
related_publications: han2024coco, wang2024exploring
---

🎉🎉 Happy to share some of our recent work about Multimodal Large Language Models. 🎉🎉



### 1️⃣ A Survey for Multimodal Reasoning

Strong Artificial Intelligence (Strong AI) or Artificial General Intelligence (AGI) with abstract reasoning ability is the goal of next-generation AI.
However, the reasoning abilities of MLLMs have not been systematically investigated. In this survey, we comprehensively review the existing evaluation protocols of multimodal reasoning, categorize and illustrate the frontiers of MLLMs, introduce recent trends in applications of MLLMs on reasoningintensive tasks, and finally discuss current practices and future directions.

<img src="{{ site.baseurl }}/assets/img/publication_preview/MLLM_reasoning_tree.png" style="zoom:40%;"/>

For more details, please refer to our 📜paper: [https://arxiv.org/abs/2401.06805](https://arxiv.org/abs/2401.06805)


### 2️⃣ Advancing Flamingo through Diverse LLM Integration

Inspired by Flamingo, we present InfiMM model series. 
This is another reproduction for Flamingo, with stronger LLMs (e.g. [LLaMA2-13B](https://ai.meta.com/llama/), [Vicuna-13B](https://huggingface.co/lmsys/vicuna-13b-v1.5), [Zephyr7B](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)), better filtering of pre-training data, and more carefully designed instruction fine-tuning.
Compared with previous open-sourced attempts ([OpenFlamingo](https://github.com/mlfoundations/open_flamingo) and [IDEFIC](https://huggingface.co/blog/idefics)), InfiMM achieves better performance on recent benchmarks (e.g., MMMU, InfiMM-Eval, MM-Vet, etc).

We achieved top performance on MMMU open-source MLLMs:

<img src="https://huggingface.co/Infi-MM/infimm-zephyr/resolve/main/assets/infimm-zephyr-mmmu-val.jpeg" style="zoom:40%;"/>

For details about our model, please refer to 🤗Huggingface: [Infi-MM/infimm-zephyr](https://huggingface.co/Infi-MM/infimm-zephyr)


### 3️⃣ Exploring Multimodal Instruction Fine-tuning

Visual instruction fine-tuning (IFT) is a vital process for aligning MLLMs’ output with user’s intentions. We noticed that models trained with LLaVA-mix-665k dataset
often struggle to follow user instructions properly in multi-round dialog. We argue that datasets with diverse and high-quality detailed instruction following annotations are essential and adequate for MLLMs IFT. In this work, we establish a new IFT dataset, with images sourced from the COCO dataset only, along with more diverse instructions. Our experiments show that when fine-tuned with our proposed dataset, MLLMs achieve better performance on open-ended evaluation benchmarks in both single-round and multi-round dialog setting.

<img src="{{ site.baseurl }}/assets/img/publication_preview/coco_all_you_need.png" style="zoom:40%;"/>

For more detals, please refer to our 📜paper: [https://arxiv.org/abs/2401.08968](https://arxiv.org/abs/2401.08968)
