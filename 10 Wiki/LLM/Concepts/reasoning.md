# Reasoning

## One-line summary

Reasoning in LLMs usually refers to the model's ability to carry out multi-step, structured, and goal-directed inference, but the term is used in many different ways.

## Why it matters

“推理能力”是今天大家最关心、也最容易说得很模糊的词之一。无论是评测、产品宣传还是实际使用，很多讨论最后都会落到 reasoning。

## Core idea

当人们说一个模型“更会推理”时，通常是在说它更擅长处理需要多步展开、约束保持、错误纠正或中间状态操作的问题。但这个词既可能指模型内部能力，也可能只是指一种更长、更稳定的输出策略。

## Key details

- reasoning 不一定意味着模型像人类一样思考
- 它可能受预训练、后训练、推理时策略和工具使用共同影响
- 数学、代码、规划和复杂问答是常见观察场景
- 很多所谓 reasoning 提升，也可能来自更好的数据和更强的解题格式

## Links

- Related:
  - [Pretraining](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/pretraining.md)
  - [Post-Training](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/post-training.md)
  - [Attention](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/attention.md)
  - [Tokenization](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/tokenization.md)
  - [In-Context Learning](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/in-context-learning.md)
- Papers:
  - `reasoning benchmarks and prompting literature`
- Models:
  - `reasoning-oriented models`
- Tools:
  - `eval suites`

## Open questions

- reasoning 到底是独立能力，还是很多已知机制叠加后的表现？
- 我们现在的 reasoning 评测，有多少在测真实泛化，有多少在测格式适配？
