---
type: acronym
full_name: Bidirectional Encoder Representations from Transformers
category:
  - NLP
aliases:
  - Bidirectional Encoder Representations from Transformers
  - 基于 Transformer 的双向编码器表示
---

# BERT

**Full Name:** Bidirectional Encoder Representations from Transformers

**中文：** 基于 Transformer 的双向编码器表示

## Definition

BERT 是基于 [[Transformer]] 编码器的预训练语言模型。它利用左右两侧的上下文表示词语，通常再针对具体 NLP 任务进行微调。

## Explanation

原始 BERT 使用掩码语言模型（[[MLM]]）和下一句预测进行预训练。它主要用于文本理解任务，不像 GPT 式模型那样逐 token 自回归生成文本；后续变体可能调整预训练目标。

## Related

- [[Transformer]]
- [[MLM]]
- [[Fine-tuning]]
- [[RoBERTa]]
- [[GPT]]

## Common Use

常用于文本分类、情感分析、[[Named Entity Recognition]]、阅读理解和抽取式问答等 NLP 任务。
