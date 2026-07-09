# Post-Training

## One-line summary

Post-training is the stage after base-model pretraining that makes a model more helpful, aligned, controllable, and usable in real tasks.

## Why it matters

很多人真正接触到的 ChatGPT 式体验，主要不是预训练直接给的，而是后训练把基础模型塑造成了更可用的产品形态。

## Core idea

预训练产生的是一个会延续文本分布的基础模型，但它不天然知道如何更好地跟随指令、拒答风险内容、维持对话风格或完成高质量任务。后训练通过监督微调、偏好优化、对齐和工具使用训练，把模型从“会续写”推向“更会协作”。

## Key details

- 常见组成包括 SFT、RLHF、DPO 或类似偏好优化
- 后训练会显著改变交互体验
- 很多安全性、语气、可控性都来自这一层
- 它也可能带来能力压缩、风格固化或过度保守

## Links

- Related:
  - [Pretraining](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/pretraining.md)
  - [Reasoning](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/reasoning.md)
  - [In-Context Learning](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/in-context-learning.md)
- Papers:
  - `alignment and preference optimization literature`
- Models:
  - `instruction-tuned models`
- Tools:
  - `evaluation pipelines`

## Open questions

- 后训练到底是在释放基础模型能力，还是也在限制它？
- 更强的推理模型有多少提升来自后训练而不是预训练？
