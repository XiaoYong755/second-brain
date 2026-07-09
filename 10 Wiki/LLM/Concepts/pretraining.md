# Pretraining

## One-line summary

Pretraining is the large-scale phase where a base language model learns general statistical structure from massive text or multimodal corpora.

## Why it matters

没有预训练，就没有后面那些“像是会思考、会写作、会解释”的基础能力。很多后续能力并不是单独教出来的，而是在预训练里先被打底。

## Core idea

在预训练阶段，模型通过自监督目标从海量数据里学习预测、压缩和表示结构。对于语言模型来说，最典型的形式就是根据前文预测下一个 token。这个阶段产出的通常是“基础模型”，能力广但不一定好用。

## Key details

- 预训练强调规模：数据规模、模型规模、算力规模
- 学到的是广泛模式，而不是任务级产品体验
- 预训练结果决定了模型的能力上限和分布偏好
- 后续的对齐、指令跟随、推理风格常建立在它之上

## Links

- Related:
  - [Tokenization](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/tokenization.md)
  - [Transformer](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/transformer.md)
  - [Post-Training](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/post-training.md)
  - [Reasoning](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/reasoning.md)
- Papers:
  - [Attention Is All You Need](/Users/taobao/Desktop/第二大脑/40%20Library/Papers/attention-is-all-you-need.md)
- Models:
  - `base models`
- Tools:
  - `training stacks`

## Open questions

- 预训练规模和后训练质量，哪个更决定最终体验？
- 数据质量与数据规模之间的拐点在哪里？
