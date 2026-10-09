---
type: acronym
full_name: Vision Transformer
category:
  - Computer Vision
aliases:
  - Vision Transformer
  - 视觉 Transformer
  - 视觉变换器
---

# ViT

**Full Name:** Vision Transformer

**中文：** 视觉 Transformer

## Definition

ViT 是一种视觉模型架构：把图像切分成 patch，并将它们作为 token 序列输入 [[Transformer]] 编码器。

## Explanation

ViT 将每个图像 patch 映射为向量，再加入位置编码；自注意力据此整合不同区域的信息。它把 Transformer 用于图像建模，可作为图像分类等任务的模型骨干，也可扩展到检测和分割。

## Related

- [[Transformer]]
- [[Self-Attention]]
- [[Patch Embedding]]
- [[CNN]]
- [[Image Classification]]

## Common Use

常见于图像分类，也可作为目标检测、图像分割及多模态系统的视觉编码器。
