# Attention

## One-line summary

Attention is the mechanism that lets a model decide which other tokens in context matter when computing the representation of the current token.

## Why it matters

很多人第一次真正理解 LLM，是从 attention 开始的。它解释了为什么模型可以在一个上下文里把前后分散的信息重新关联起来。

## Core idea

给定一个 token，模型不会一视同仁地看待上下文里的其他 token，而是会学会给不同位置分配不同权重。attention 本质上是一种“按需读取上下文”的机制，它决定当前计算时应该更关注哪里。

## Key details

- self-attention 是 Transformer 里的关键部件
- 不同 attention head 往往会学到不同的模式
- attention 不是“理解”的完整解释，但它是重要的可观察窗口
- 长上下文性能、推理速度和内存开销都和 attention 设计强相关

## Links

- Related:
  - [Transformer](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/transformer.md)
  - [Tokenization](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/tokenization.md)
  - [Reasoning](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/reasoning.md)
  - [In-Context Learning](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/in-context-learning.md)
- Papers:
  - [Attention Is All You Need](/Users/taobao/Desktop/第二大脑/40%20Library/Papers/attention-is-all-you-need.md)
- Models:
  - `Transformer-based models`
- Tools:
  - `attention visualizers`

## Open questions

- attention 权重到底在多大程度上能解释模型行为？
- 更高效的 attention 变体会怎样改变 LLM 的实际使用边界？
