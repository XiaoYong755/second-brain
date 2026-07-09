# Transformer

## One-line summary

The Transformer is the neural network architecture that powers most modern language models by using attention instead of recurrence to process token sequences.

## Why it matters

如果说现代 LLM 有一块最核心的计算骨架，那基本就是 Transformer。很多后来的模型变化，都是在它的基础上做扩展、缩减、加速或对齐。

## Core idea

Transformer 不再像 RNN 那样按时间步一步一步处理序列，而是把一个上下文窗口里的 token 一起送进网络，通过 attention 让每个位置都能有条件地参考其他位置。这样既更容易并行训练，也更适合捕捉长距离依赖。

## Key details

- 它最早在机器翻译语境里提出，但后来成了语言模型主干
- self-attention 是它的核心机制之一
- 位置编码或位置表示解决“顺序信息”问题
- 大多数 LLM 主要使用 decoder-only Transformer 变体

## Links

- Related:
  - [Attention](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/attention.md)
  - [Tokenization](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/tokenization.md)
  - [Pretraining](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/pretraining.md)
  - [In-Context Learning](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/in-context-learning.md)
- Papers:
  - [Attention Is All You Need](/Users/taobao/Desktop/第二大脑/40%20Library/Papers/attention-is-all-you-need.md)
- Models:
  - `GPT-style models`
- Tools:
  - `transformer libraries`

## Open questions

- 哪些 LLM 能力来自 Transformer 本身，哪些更像是规模和数据带来的涌现？
- 如果未来主流架构变化，哪些部分会被保留？
