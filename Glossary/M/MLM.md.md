---
type: acronym
full_name: Masked Language Modeling
category:
  - NLP
aliases:
  - Masked Language Modeling
  - Masked LM
  - 掩码语言建模
---

# MLM

**Full Name:** Masked Language Modeling

**中文：** 掩码语言建模

## Definition

MLM 是一种预训练目标：随机遮盖输入中的部分 token，让模型根据其余上下文预测被遮盖的原词。

## Explanation

被遮盖位置两侧的上下文都可用于预测，因此 MLM 能训练编码器式模型学习双向语言表示。它是 [[BERT]]、[[RoBERTa]] 等模型使用的经典预训练目标；原始 BERT 还搭配了下一句预测任务。

## Related

- [[BERT]]
- [[RoBERTa]]
- [[Transformer]]
- [[Causal Language Modeling]]

## Common Use

常用于 NLP 编码器模型的预训练，尤其是文本分类、信息抽取等理解任务的模型。
