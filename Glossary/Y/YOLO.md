---
type: acronym
full_name: You Only Look Once
category:
  - Computer Vision
aliases:
  - You Only Look Once
  - YOLO 系列
---

# YOLO

**Full Name:** You Only Look Once

**中文：** 只看一次

## Definition

YOLO 是一系列单阶段目标检测模型。图像经过一次网络前向计算，就能得到候选目标的位置、类别和分数。

## Explanation

原版 YOLO 直接从整张图像预测边界框和类别概率。这就是名称里「只看一次」的含义。一次前向计算得到的是预测结果，部分版本还会用非极大值抑制（[[NMS]]）去除重复框。[原论文](https://openaccess.thecvf.com/content_cvpr_2016/html/Redmon_You_Only_Look_CVPR_2016_paper.html)

## Related

- [[Object Detection]]
- [[Bounding Box]]
- [[NMS]]
- [[SAM]]

## Common Use

常用于视频目标检测和工业视觉。需要像素级轮廓时，可以把 YOLO 检测到的边界框作为 [[SAM]] 的提示，生成对应的分割掩码。
