---
type: acronym
full_name: Stochastic Gradient Descent
category:
  - Training
aliases:
  - Stochastic Gradient Descent
  - 随机梯度下降
---

# SGD

**Full Name:** Stochastic Gradient Descent

**中文：** 随机梯度下降

## Definition

SGD 是一种优化算法：随机抽取训练样本来估计损失函数的梯度，再沿负梯度方向更新模型参数。

## Explanation

严格意义上的 SGD 每次使用一个样本；深度学习中通常使用 [[Mini-batch]]，也常统称为 SGD。相比每次用全部训练数据计算梯度，它减少单步计算量，但梯度估计更有噪声。[[Learning Rate]] 控制更新幅度，SGD 也常配合 [[Momentum]] 使用。

## Related

- [[Gradient Descent]]
- [[Mini-batch]]
- [[Learning Rate]]
- [[Momentum]]
- [[Adam]]

## Common Use

常用于线性模型和神经网络训练；在 [[CNN]]、图像分类等训练配置中，经常可以看到带 Momentum 的 SGD。
