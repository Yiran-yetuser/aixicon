---
type: acronym
full_name: Segment Anything Model
category:
  - Computer Vision
aliases:
  - Segment Anything Model
  - Segment Anything
  - 分割一切模型
---

# SAM

**Full Name:** Segment Anything Model

**中文：** 分割一切模型

## Definition

SAM 是一种可提示的图像分割模型。给定一张图和点、边界框或已有掩码等提示，它会输出对应区域的像素级分割掩码。

## Explanation

原版 SAM 用 [[ViT]] 编码图像，再由提示编码器和掩码解码器结合图像特征与提示来预测掩码。同一张图的特征可以复用，换一个提示就能分割另一个区域。[原论文](https://openaccess.thecvf.com/content/ICCV2023/papers/Kirillov_Segment_Anything_ICCV_2023_paper.pdf)

## Related

- [[ViT]]
- [[Image Segmentation]]
- [[Object Detection]]

## Common Use

常用于交互式标注和图像编辑，也可以接收目标检测器输出的边界框，为检测到的目标生成掩码。

在模型训练文献中，SAM 也可指优化方法 Sharpness-Aware Minimization。[优化方法原论文](https://arxiv.org/abs/2010.01412)
