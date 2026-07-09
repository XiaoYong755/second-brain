# Attention Is All You Need

## Citation

- authors: Ashish Vaswani et al.
- year: 2017
- link: https://arxiv.org/abs/1706.03762

## One-line summary

This paper introduced the Transformer architecture, replacing recurrence with attention-based sequence modeling.

## What problem it solves

在序列建模里，RNN 类架构难以并行、长距离依赖也更难处理。Transformer 用 attention 机制重构了这个问题。

## Main contribution

- 提出 Transformer
- 把 self-attention 作为核心计算机制
- 大幅提升并行训练能力
- 为后来的大语言模型打下基础

## My understanding

这篇论文的重要性不只是“提出了一个新架构”，而是重新定义了现代语言模型的计算骨架。今天几乎所有主流 LLM 都可以往回追溯到它。

## Related wiki pages

- [In-Context Learning](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/in-context-learning.md)
- `attention`
- `transformer`
