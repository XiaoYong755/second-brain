# Tokenization

## One-line summary

Tokenization is the process of turning raw text into discrete units that a language model can process and generate.

## Why it matters

很多初学者会把模型理解成“直接读字”，但模型真正处理的是 token。上下文长度、成本、分词边界、甚至一些奇怪行为，往往都和 tokenization 有直接关系。

## Core idea

语言模型不能直接对自然语言字符串做计算，它需要先把文本映射成离散 token，再把 token 映射成向量。tokenization 是文本世界和模型计算世界之间的接口层。

## Key details

- token 不等于单词，也不等于字符
- 常见方法包括 BPE、SentencePiece 等
- 不同 tokenizer 会影响上下文利用效率
- 多语言、代码、符号和格式化文本会带来不同的分词挑战

## Links

- Related:
  - [Transformer](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/transformer.md)
  - [Pretraining](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/pretraining.md)
  - [Reasoning](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/Concepts/reasoning.md)
- Papers:
  - [Attention Is All You Need](/Users/taobao/Desktop/第二大脑/40%20Library/Papers/attention-is-all-you-need.md)
- Models:
  - `GPT-style models`
- Tools:
  - `tokenizers`

## Open questions

- 对代码和多模态输入来说，最好的 token 表示应该长什么样？
- 未来更强的模型会不会弱化 tokenizer 设计的重要性？
