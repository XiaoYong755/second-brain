# In-Context Learning

## One-line summary

In-context learning is the ability of a language model to adapt its behavior from examples or instructions placed inside the prompt, without updating model weights.

## Why it matters

这是 LLM 和传统监督学习体验差异最大的地方之一。很多“像是在临时学会一件事”的表现，本质上都和它有关。

## Core idea

模型在预训练阶段学会了一种通用的模式匹配和条件生成能力。推理时，我们通过提示词、示例、格式约束、角色设定等上下文，把任务描述进输入里，模型就能在不训练的前提下表现出任务适配能力。

## Key details

- 它不等于真正在线学习，但会表现出某种“上下文内任务适配”
- few-shot prompting 是典型表现形式
- instruction following 也常和它联动出现
- 上下文窗口大小、训练数据分布、模型规模都会影响效果

## Links

- Related:
  - `attention`
  - `transformer`
  - `prompting`
- Papers:
  - [Attention Is All You Need](/Users/taobao/Desktop/第二大脑/40%20Library/Papers/attention-is-all-you-need.md)
- Models:
  - `GPT-style models`
- Tools:
  - `prompt playgrounds`

## Open questions

- 它到底更像“隐式检索”还是“临时程序执行”？
- 不同模型的 in-context learning 上限主要由什么决定？
